####1,dart语言特性中的循环语句定义和操作方法
####2,dart字符串的定义和操作方法
####3,dart函数定义和使用方法
####4,dart中数组定义和使用方法
#### 5.dart中列表定义和使用方法
Lists use zero-based indexing, where 0 is the index of the first element and list.length - 1 is the index of the last element.
```var list = [1, 2, 3];
list[1] = 1;```
#### 6.dart中 Map定义和使用方法
```var gifts = {                  //图// Keys     
 Values  'first' : 'partridge',  'second': 'turtledoves',  'fifth' : 'golden rings'};
var nobleGases = {// Keys 
Values  2 :   'helium',  10:   'neon',  18:   'argon',};```
#### 7. querySelector（）函数的详细API解释
https://api.dartlang.org/stable/1.19.1/dart-html/querySelector.html
``` var element1 = document.querySelector('.className');
var element2 = document.querySelector('#id');```
```Element querySelector(String selectors) => document.querySelector(selectors);  //source```
#### 8. 详细解释dart如何操作html的文档
##### Edit the HTML source codeClick HTML, at the upper left of DartPad. The view switches from Dart code to the (non-existent) HTML code.Add the following HTML code:
```<p id="RipVanWinkle">  RipVanWinkle paragraph.</p>```
Click HTML OUTPUT to see how a browser would render your HTML.
##### Edit the Dart source codeClick DART, at the upper right of DartPad. The view switches from HTML code to Dart code.Change the Dart code to the following:
```import 'dart:html';
void main() { 
querySelector('#RipVanWinkle').text = 'Wake up, sleepy head!';
}```
Click Run to execute your code.The text in the HTML OUTPUT tab changes to “Wake up, sleepy head!”

####9,dart web app 应用程序组织结构的解释部分
####10, dart可用的各种工具的解释部分
####11,指引你到其他社区社区寻求dart相关问题帮助的解释部分
####12,从web storm软件菜单找出webstrom 中dart开发的帮助文档
