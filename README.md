### JavaVerbalExpressions
---
https://github.com/VerbalExpressions/JavaVerbalExpressions

```java
VerbalExpression testRegex = VerbalExpression.regex()
    .startOfLine().then("http").maybe("s")
    .then("://")
    .maybe("www.").anythingBut(" ")
    .endOfLine()
    .build();

String url = "https://www.google.com";
testRegex.testExact(url);
testRegex.toString();

VarbalExpression testRegex = VerbalExpression.regex()
    .startOfLine().then("abc").or("def")
    .build();
String testString = "defzzz";
testRegex.test(testString);
testRegex.testExact(testString);
testRegex.getText(testString);

VarbalExpression regex = regex(regex().anything().addModifier('i')).endOfLine().build();
VerbalExpression.Builder digits = regex().capt().digit().oneOrMore().endCapt().tab();
VerbalExpression regex2 = regex().add(digits).add(digits).build();

regex().wordChar().nonWordChar()
  .space().nonSpace()
  .digit().nonDigit()
  
String text = "aaabcd";
VerbalExpression regex = regex()
    .find("a")
    .capture().find("b").anything().endCapture().then("cd").build();

regex.getText(text)
regex.getText(text, 1)

```

```
```

```
```


