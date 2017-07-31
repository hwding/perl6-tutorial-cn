# Perl6 入门指导
<img height="64" width="64" src="https://perl6.org/camelia-logo.png" ></img>  
译自 [The-Perl-Maven's-Perl-6-Tutorial](http://perl6maven.com/tutorial/toc)

## 关于此翻译
译文对原文表达不当之处做了适当的修改，在表达不清晰之处提供了译注，并优化了部分排版。  
另外，由于历史原因原文中的部分内容可能出现因过时而导致的错误，在翻译时也会做相应的修正并附以译注。  
对原文以及代码的修正会以PR的形式提交到网站镜像[szabgab/perl6maven.com](https://github.com/szabgab/perl6maven.com/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Ahwding)。  

## 关于原作者
欢迎关注原作者[Gabor Szabo](https://github.com/szabgab)的新框架[Bailador](https://github.com/Bailador/Bailador)以及新书[*Web Application Development in Perl 6*](https://leanpub.com/bailador)

## 总目录
### [第一章 初探Perl6](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E7%AC%AC%E4%B8%80%E7%AB%A0-%E5%88%9D%E6%8E%A2perl6)
- [Hello World - 标量变量](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#hello-world---%E6%A0%87%E9%87%8F%E5%8F%98%E9%87%8F)
- [Hello World - 嵌入变量](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#hello-world---%E5%B5%8C%E5%85%A5%E5%8F%98%E9%87%8F)
- [读取键盘输入](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E8%AF%BB%E5%8F%96%E9%94%AE%E7%9B%98%E8%BE%93%E5%85%A5)
- [数字运算符](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E6%95%B0%E5%AD%97%E8%BF%90%E7%AE%97%E7%AC%A6)
- [将字符串自动转换为数字](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E5%B0%86%E5%AD%97%E7%AC%A6%E4%B8%B2%E8%87%AA%E5%8A%A8%E8%BD%AC%E6%8D%A2%E4%B8%BA%E6%95%B0%E5%AD%97)
- [字符串运算符](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E5%AD%97%E7%AC%A6%E4%B8%B2%E8%BF%90%E7%AE%97%E7%AC%A6)
- [字符串的拼接](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E5%AD%97%E7%AC%A6%E4%B8%B2%E7%9A%84%E6%8B%BC%E6%8E%A5)
- [字符串的反复](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E5%AD%97%E7%AC%A6%E4%B8%B2%E7%9A%84%E5%8F%8D%E5%A4%8D)
- [`if`语句 - 值的比较](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#if%E8%AF%AD%E5%8F%A5---%E5%80%BC%E7%9A%84%E6%AF%94%E8%BE%83)
- [三元运算符](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E4%B8%89%E5%85%83%E8%BF%90%E7%AE%97%E7%AC%A6)
- [比较运算符](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E6%AF%94%E8%BE%83%E8%BF%90%E7%AE%97%E7%AC%A6)
- [布尔表达式(逻辑运算符)](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E5%B8%83%E5%B0%94%E8%A1%A8%E8%BE%BE%E5%BC%8F%E9%80%BB%E8%BE%91%E8%BF%90%E7%AE%97%E7%AC%A6)
- [链式比较](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E9%93%BE%E5%BC%8F%E6%AF%94%E8%BE%83)
- [一个简易计算器 - 使用值的比较](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E4%B8%80%E4%B8%AA%E7%AE%80%E6%98%93%E8%AE%A1%E7%AE%97%E5%99%A8---%E4%BD%BF%E7%94%A8%E5%80%BC%E7%9A%84%E6%AF%94%E8%BE%83)
- [一个简易计算器 - 使用given语句](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E4%B8%80%E4%B8%AA%E7%AE%80%E6%98%93%E8%AE%A1%E7%AE%97%E5%99%A8---%E4%BD%BF%E7%94%A8given%E8%AF%AD%E5%8F%A5)
- [string类型方法：`index`](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#string%E7%B1%BB%E5%9E%8B%E6%96%B9%E6%B3%95index)
- [string类型方法：`substr`](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#string%E7%B1%BB%E5%9E%8B%E6%96%B9%E6%B3%95substr)
- ["超级"`or`(条件联结)](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E8%B6%85%E7%BA%A7or%E6%9D%A1%E4%BB%B6%E8%81%94%E7%BB%93)
### [第二章 元运算符](https://github.com/hwding/perl6-doc-cn/blob/master/CH02.md#%E7%AC%AC%E4%BA%8C%E7%AB%A0-%E5%85%83%E8%BF%90%E7%AE%97%E7%AC%A6)
- [什么是元运算符](https://github.com/hwding/perl6-doc-cn/blob/master/CH02.md#%E4%BB%80%E4%B9%88%E6%98%AF%E5%85%83%E8%BF%90%E7%AE%97%E7%AC%A6)
- [赋值运算符](https://github.com/hwding/perl6-doc-cn/blob/master/CH02.md#%E8%B5%8B%E5%80%BC%E8%BF%90%E7%AE%97%E7%AC%A6)
- [在赋值时调用方法](https://github.com/hwding/perl6-doc-cn/blob/master/CH02.md#%E5%9C%A8%E8%B5%8B%E5%80%BC%E6%97%B6%E8%B0%83%E7%94%A8%E6%96%B9%E6%B3%95)
- [在赋值时调用函数](https://github.com/hwding/perl6-doc-cn/blob/master/CH02.md#%E5%9C%A8%E8%B5%8B%E5%80%BC%E6%97%B6%E8%B0%83%E7%94%A8%E5%87%BD%E6%95%B0)
- [否定关系运算符](https://github.com/hwding/perl6-doc-cn/blob/master/CH02.md#%E5%90%A6%E5%AE%9A%E5%85%B3%E7%B3%BB%E8%BF%90%E7%AE%97%E7%AC%A6)
- [反转运算符](https://github.com/hwding/perl6-doc-cn/blob/master/CH02.md#%E5%8F%8D%E8%BD%AC%E8%BF%90%E7%AE%97%E7%AC%A6)
- [超算符](https://github.com/hwding/perl6-doc-cn/blob/master/CH02.md#%E8%B6%85%E7%AE%97%E7%AC%A6)
- [归约运算符](https://github.com/hwding/perl6-doc-cn/blob/master/CH02.md#%E5%BD%92%E7%BA%A6%E8%BF%90%E7%AE%97%E7%AC%A6)
- [归约三角运算符](https://github.com/hwding/perl6-doc-cn/blob/master/CH02.md#%E5%BD%92%E7%BA%A6%E4%B8%89%E8%A7%92%E8%BF%90%E7%AE%97%E7%AC%A6)
- [交叉运算符](https://github.com/hwding/perl6-doc-cn/blob/master/CH02.md#%E4%BA%A4%E5%8F%89%E8%BF%90%E7%AE%97%E7%AC%A6)
### [第三章 Perl6中的联结](https://github.com/hwding/perl6-doc-cn/blob/master/CH03.md#perl6%E4%B8%AD%E7%9A%84%E8%81%94%E7%BB%93)
- [联结](https://github.com/hwding/perl6-doc-cn/blob/master/CH03.md#%E8%81%94%E7%BB%93)
- [更多关于联结的练习](https://github.com/hwding/perl6-doc-cn/blob/master/CH03.md#%E6%9B%B4%E5%A4%9A%E5%85%B3%E4%BA%8E%E8%81%94%E7%BB%93%E7%9A%84%E7%BB%83%E4%B9%A0)
### [第四章 Perl6文件操作](https://github.com/hwding/perl6-doc-cn/blob/master/CH04.md#perl6%E6%96%87%E4%BB%B6%E6%93%8D%E4%BD%9C)
- [`exit()`](https://github.com/hwding/perl6-doc-cn/blob/master/CH04.md#exit)
- [`warn()`](https://github.com/hwding/perl6-doc-cn/blob/master/CH04.md#warn)
- [`die()`](https://github.com/hwding/perl6-doc-cn/blob/master/CH04.md#die)
- [Twigils与特殊变量](https://github.com/hwding/perl6-doc-cn/blob/master/CH04.md#twigils%E4%B8%8E%E7%89%B9%E6%AE%8A%E5%8F%98%E9%87%8F)
- [读取文件](https://github.com/hwding/perl6-doc-cn/blob/master/CH04.md#%E8%AF%BB%E5%8F%96%E6%96%87%E4%BB%B6)
- [使用`get()`读取所有行](https://github.com/hwding/perl6-doc-cn/blob/master/CH04.md#%E4%BD%BF%E7%94%A8get%E8%AF%BB%E5%8F%96%E6%89%80%E6%9C%89%E8%A1%8C)
- [逐行读取文件](https://github.com/hwding/perl6-doc-cn/blob/master/CH04.md#%E9%80%90%E8%A1%8C%E8%AF%BB%E5%8F%96%E6%96%87%E4%BB%B6)
- [写文件](https://github.com/hwding/perl6-doc-cn/blob/master/CH04.md#%E5%86%99%E6%96%87%E4%BB%B6)
- [文件模式](https://github.com/hwding/perl6-doc-cn/blob/master/CH04.md#%E6%96%87%E4%BB%B6%E6%A8%A1%E5%BC%8F)
- [`slurp()`与`spurt()`](https://github.com/hwding/perl6-doc-cn/blob/master/CH04.md#slurp%E4%B8%8Espurt)
- [将文件逐行读取至数组](https://github.com/hwding/perl6-doc-cn/blob/master/CH04.md#%E5%B0%86%E6%96%87%E4%BB%B6%E9%80%90%E8%A1%8C%E8%AF%BB%E5%8F%96%E8%87%B3%E6%95%B0%E7%BB%84)
- [练习：利用文件IO计算其中数字的和](https://github.com/hwding/perl6-doc-cn/blob/master/CH04.md#%E7%BB%83%E4%B9%A0%E5%88%A9%E7%94%A8%E6%96%87%E4%BB%B6io%E8%AE%A1%E7%AE%97%E5%85%B6%E4%B8%AD%E6%95%B0%E5%AD%97%E7%9A%84%E5%92%8C)
- [答案：利用文件IO计算其中数字的和](https://github.com/hwding/perl6-doc-cn/blob/master/CH04.md#%E7%AD%94%E6%A1%88%E5%88%A9%E7%94%A8%E6%96%87%E4%BB%B6io%E8%AE%A1%E7%AE%97%E5%85%B6%E4%B8%AD%E6%95%B0%E5%AD%97%E7%9A%84%E5%92%8C)
### [第五章 Perl6列表与数组](https://github.com/hwding/perl6-doc-cn/blob/master/CH05.md#perl6%E5%88%97%E8%A1%A8%E4%B8%8E%E6%95%B0%E7%BB%84)
- [列表字面量](https://github.com/hwding/perl6-doc-cn/blob/master/CH05.md#%E5%88%97%E8%A1%A8%E5%AD%97%E9%9D%A2%E9%87%8F)
- [列表赋值](https://github.com/hwding/perl6-doc-cn/blob/master/CH05.md#%E5%88%97%E8%A1%A8%E8%B5%8B%E5%80%BC)
- [交换两个变量](https://github.com/hwding/perl6-doc-cn/blob/master/CH05.md#%E4%BA%A4%E6%8D%A2%E4%B8%A4%E4%B8%AA%E5%8F%98%E9%87%8F)
- [使用`for`循环遍历列表元素](https://github.com/hwding/perl6-doc-cn/blob/master/CH05.md#%E4%BD%BF%E7%94%A8for%E5%BE%AA%E7%8E%AF%E9%81%8D%E5%8E%86%E5%88%97%E8%A1%A8%E5%85%83%E7%B4%A0)
- [建立数组并遍历之](https://github.com/hwding/perl6-doc-cn/blob/master/CH05.md#%E5%BB%BA%E7%AB%8B%E6%95%B0%E7%BB%84%E5%B9%B6%E9%81%8D%E5%8E%86%E4%B9%8B)
- [数组元素（创建目录）](https://github.com/hwding/perl6-doc-cn/blob/master/CH05.md#%E6%95%B0%E7%BB%84%E5%85%83%E7%B4%A0%E5%88%9B%E5%BB%BA%E7%9B%AE%E5%BD%95)
- [数组赋值](https://github.com/hwding/perl6-doc-cn/blob/master/CH05.md#%E6%95%B0%E7%BB%84%E8%B5%8B%E5%80%BC)
- [命令行选项](https://github.com/hwding/perl6-doc-cn/blob/master/CH05.md#%E5%91%BD%E4%BB%A4%E8%A1%8C%E9%80%89%E9%A1%B9)
- [处理CSV文件](https://github.com/hwding/perl6-doc-cn/blob/master/CH05.md#%E5%A4%84%E7%90%86csv%E6%96%87%E4%BB%B6)
- [联结](https://github.com/hwding/perl6-doc-cn/blob/master/CH05.md#%E8%81%94%E7%BB%93)
- [`unique`函数](https://github.com/hwding/perl6-doc-cn/blob/master/CH05.md#unique%E5%87%BD%E6%95%B0)
- [单值遍历](https://github.com/hwding/perl6-doc-cn/blob/master/CH05.md#%E5%8D%95%E5%80%BC%E9%81%8D%E5%8E%86)
- [多值遍历](https://github.com/hwding/perl6-doc-cn/blob/master/CH05.md#%E5%A4%9A%E5%80%BC%E9%81%8D%E5%8E%86)
- [缺少列表项](https://github.com/hwding/perl6-doc-cn/blob/master/CH05.md#%E7%BC%BA%E5%B0%91%E5%88%97%E8%A1%A8%E9%A1%B9)
- [同时遍历多个数组](https://github.com/hwding/perl6-doc-cn/blob/master/CH05.md#%E5%90%8C%E6%97%B6%E9%81%8D%E5%8E%86%E5%A4%9A%E4%B8%AA%E6%95%B0%E7%BB%84)
- [`Z`即`zip`](https://github.com/hwding/perl6-doc-cn/blob/master/CH05.md#z%E5%8D%B3zip)
- [`xx` - 字符串倍率器](https://github.com/hwding/perl6-doc-cn/blob/master/CH05.md#xx%E5%AD%97%E7%AC%A6%E4%B8%B2%E5%80%8D%E7%8E%87%E5%99%A8)
- [排序](https://github.com/hwding/perl6-doc-cn/blob/master/CH05.md#%E6%8E%92%E5%BA%8F)
- [使用`map`变换数组和列表](https://github.com/hwding/perl6-doc-cn/blob/master/CH05.md#%E4%BD%BF%E7%94%A8map%E5%8F%98%E6%8D%A2%E6%95%B0%E7%BB%84%E5%92%8C%E5%88%97%E8%A1%A8)
### [第六章 Perl6散列](https://github.com/hwding/perl6-doc-cn/blob/master/CH06.md#perl6%E6%95%A3%E5%88%97)
- [散列（哈希/联合数组）](https://github.com/hwding/perl6-doc-cn/blob/master/CH06.md#%E6%95%A3%E5%88%97%E5%93%88%E5%B8%8C%E8%81%94%E5%90%88%E6%95%B0%E7%BB%84)
- [从散列中取值](https://github.com/hwding/perl6-doc-cn/blob/master/CH06.md#%E4%BB%8E%E6%95%A3%E5%88%97%E4%B8%AD%E5%8F%96%E5%80%BC)
- [多维散列](https://github.com/hwding/perl6-doc-cn/blob/master/CH06.md#%E5%A4%9A%E7%BB%B4%E6%95%A3%E5%88%97)
- [词频统计](https://github.com/hwding/perl6-doc-cn/blob/master/CH06.md#%E8%AF%8D%E9%A2%91%E7%BB%9F%E8%AE%A1)
- [散列用法总览](https://github.com/hwding/perl6-doc-cn/blob/master/CH06.md#%E6%95%A3%E5%88%97%E7%94%A8%E6%B3%95%E6%80%BB%E8%A7%88)
- [“啜食”散列](https://github.com/hwding/perl6-doc-cn/blob/master/CH06.md#%E5%95%9C%E9%A3%9F%E6%95%A3%E5%88%97)
- [取出所有的键值对](https://github.com/hwding/perl6-doc-cn/blob/master/CH06.md#%E5%8F%96%E5%87%BA%E6%89%80%E6%9C%89%E7%9A%84%E9%94%AE%E5%80%BC%E5%AF%B9)
- [取出所有的键](https://github.com/hwding/perl6-doc-cn/blob/master/CH06.md#%E5%8F%96%E5%87%BA%E6%89%80%E6%9C%89%E7%9A%84%E9%94%AE)
### 第七章 Perl5 to Perl6
- Intro
- Hello World
- Scalars
- Arrays
- Hashes
- Control Structures
- Functions
- Files
- Modules, Classes
- Perl 5 to Perl 6
### 第八章 Testing in Perl6
- skip a test
### 第九章 Object Oriented Perl6
- Simple Point class
- Read/write attributes and accessors
- Class Methods
- Private Attributes
- Method with parameters
- Inheritence of classes
- Classes in Perl 6
### 第十章 Perl6 Regexes
- Regexes in Perl 6
- Match digit
- Match Any character
- Escape characters
- Spaces in regex
- End of string anchors
- Ranges
- Regex Arithmetic
- Regex Quantifier
- Quantifier 2
- Match several words
- Alternates
- Match object
- Capture
- Named Regex
- Capture with quantifier
- Reuse capture
- Word boundary
- Rules
- Tokens
- Replace
- Grammar
- Grammar with error handling
- Grammar that is easier to extend
- Grammar subclass
### 第十一章 Shell to Perl6
- Intro
- Running external command from Perl 6 (shell, QX)
- Unix commands in Perl 6
- awk
- cat
- cd in Perl 6
- chmod
- chown
- cmp
- compress
- cut
- date
- diff
- df
- dos2unix
- du
- file
- find
- grep
- gzip
- head
- kill
- ln
- ls or dir in Perl 6
- mkdir
- mv
- ps
- popd
- pushd
- Current Working Directory in Perl 6 (cwd, pwd, $*CWD)
- rmdir
- rm
- sed
- sort
- tail
- tar
- touch
- uniq
- unix2dos
- wc
- who
- zip
- Other UNIX command
### 第十二章 Appendix
- grok and App::Grok
- Using 3rd party Perl 6 modules
- Timestamp and elapsed time in Perl 6
- Thanks
### 第十三章 Introduction to Perl6
- Getting started
- Other resources
- Installing Rakudo Perl 6
- Development Environment
- Running Rakudo
- Hello World
- Comments
- POD - Plain Old Documentation
### 第十四章 Subroutines
- Subroutines in Perl 6
- Simple definition with required parameters
- Subroutine with arbitrary number of parameters
- Passing arrays and hashes
- Multiple signatures
- Optional parameters
- Named only parameters
- No parameter definition - perl 5 style
- Fibonacci
- Creating Operators
- Create your own operator
### 第十五章 Modules in Perl6
- Exporting subs from modules
