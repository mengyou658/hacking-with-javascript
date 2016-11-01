# 当心隐形的强制转换

```javascript
```
[示例](item3/demo.js)

-----
谨记:
+ 强制转换可能会导致隐形的类型错误。
+ `+`号运算符会根据它的参数类型来决定是做加法还是字符串的拼接。
+ `Object`通过它的`toString`方法被强制转换为字符串,通过它的`valueOf`方法被强制转换为数字。
+ 带有`valueOf`方法的`Object`应该实现一个`toString`方法,这个`toString`方法返回的字符串就是那个`valueOf`返回的数字的字符串表示形式。
+ 判断一个值是否是未定义的应该使用`typeof`或者比较的方法,而不是根据这个值表现是`true`或者`false`来判断。