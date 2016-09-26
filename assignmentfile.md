#### 1,dart语言特性中的循环语句定义和操作方法
``` dart
(1)for (int month = 1; month <= 12; month++) {
  print(month);
}
（2）while (year < 2016) {
  year += 1;
}
```
#### 2,dart字符串的定义和操作方法
``` dart 
（1）	String name = 'Bob';
（2）	var s1 = 'Single quotes work well for string literals.';
```
#### 3,dart函数定义和使用方法
``` dart
（1）int fibonacci(int n) {
      if (n == 0 || n == 1) return n;
      return fibonacci(n - 1) + fibonacci(n - 2);
}
var result = fibonacci(20);
（3）	flybyObjects.where((name) => name.contains('anus')).forEach(print);
```
#### 4,dart中数组定义和使用方法
根据官网资料显示，dart中数组的使用与列表相似 
#### 5.dart中列表定义和使用方法
Lists use zero-based indexing, where 0 is the index of the first element and list.length - 1 is the index of the last element.
```var list = [1, 2, 3];
list[1] = 1;
```

#### 6.dart中 Map定义和使用方法
``` var gifts = {                  //图// Keys     
 Values  'first' : 'partridge',  'second': 'turtledoves',  'fifth' : 'golden rings'};
var nobleGases = {// Keys 
Values  2 :   'helium',  10:   'neon',  18:   'argon',};
```
#### 7. querySelector（）函数的详细API解释
https://api.dartlang.org/stable/1.19.1/dart-html/querySelector.html
``` var element1 = document.querySelector('.className');
var element2 = document.querySelector('#id');
```
```Element querySelector(String selectors) => document.querySelector(selectors);  //source
```
#### 8. 详细解释dart如何操作html的文档
##### Edit the HTML source codeClick HTML, at the upper left of DartPad. The view switches from Dart code to the (non-existent) HTML code.Add the following HTML code:
```<p id="RipVanWinkle">  RipVanWinkle paragraph.</p>
```
Click HTML OUTPUT to see how a browser would render your HTML.
##### Edit the Dart source codeClick DART, at the upper right of DartPad. The view switches from HTML code to Dart code.Change the Dart code to the following:
```import 'dart:html';
void main() { 
querySelector('#RipVanWinkle').text = 'Wake up, sleepy head!';
}
```
Click Run to execute your code.The text in the HTML OUTPUT tab changes to “Wake up, sleepy head!”

####9. dart web app 应用程序组织结构的解释部分
  以下是dart web app项目目录结构
```+web 
 +packages 
 +dart 
 +style 
  index.html 
```
web目录是整个web程序的根目录，index.html就是我们的入口文件，style目录中存放css样式文件，dart目录中存放的是dart文件， 而packages目录中存放的是dart语言的libraries，比如说我们希望使用dart:html库，那么就是加载了packages目录下的该库文件。
.packages文件描述了库与文件路径的对应关系

#####10. dart可用的各种工具的解释部分
#####IDEs
dart语言的插件已经被许多常用的IDE （像webstorm等）所支持; 
当然也可以为一些文本编辑器（像vim、sublimetext等）安装dart的插件
#####SDKs
用途	sdk
web app(移动端的web页面)、作为脚本或服务器	dart
移动端原生app	Flutter
命令行工具
pub 包管理工具
管理Dart的包，用于安装，使用和分享Dart库，支持Dart插件的IDEs对pub都有支持；
#####静态分析器
运行并报告你的代码中的任何的错误和警告。你的IDE的这个Dart插件应当利用了Dart的解释引擎，但是你也自己在命令行中运行这个分析器
代码规范器
规范你的代码格式，按照dart风格规范的要求，你的IDE通常就会允许你来规范化你的代码风格。

####11.指引你到其他社区社区寻求dart相关问题帮助的解释部分
   Get help区块：
   
       有许多我们可以回答或者问dart相关问题的平台和社区，在Community and Support这一块。

####12.从web storm软件菜单找出webstrom 中dart开发的帮助文档
   https://www.jetbrains.com/help/webstorm/2016.2/dart-support.html?search=dart
