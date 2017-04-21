# Perl6 入门指导
<img height="64" width="64" src="https://perl6.org/camelia-logo.png" ></img>  
翻译自 The-Perl-Maven's-Perl-6-Tutorial: http://perl6maven.com/tutorial/toc.
## 关于
译： [hwding](https://github.com/hwding) <<m@amastigote.com>>  
仅供学习参考，不恰之处敬请指正。  
译文对原文表达不当之处做了适当的修改，在表达不清晰之处提供了译注，并优化了部分排版。

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
- [if语句 - 值的比较](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#if%E8%AF%AD%E5%8F%A5---%E5%80%BC%E7%9A%84%E6%AF%94%E8%BE%83)
- [三元运算符](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E4%B8%89%E5%85%83%E8%BF%90%E7%AE%97%E7%AC%A6)
- [比较运算符](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E6%AF%94%E8%BE%83%E8%BF%90%E7%AE%97%E7%AC%A6)
- [布尔表达式(逻辑运算符)](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E5%B8%83%E5%B0%94%E8%A1%A8%E8%BE%BE%E5%BC%8F%E9%80%BB%E8%BE%91%E8%BF%90%E7%AE%97%E7%AC%A6)
- [链式比较](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E9%93%BE%E5%BC%8F%E6%AF%94%E8%BE%83)
- [一个简易计算器 - 使用值的比较](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E4%B8%80%E4%B8%AA%E7%AE%80%E6%98%93%E8%AE%A1%E7%AE%97%E5%99%A8---%E4%BD%BF%E7%94%A8%E5%80%BC%E7%9A%84%E6%AF%94%E8%BE%83)
- [一个简易计算器 - 使用given语句](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E4%B8%80%E4%B8%AA%E7%AE%80%E6%98%93%E8%AE%A1%E7%AE%97%E5%99%A8---%E4%BD%BF%E7%94%A8given%E8%AF%AD%E5%8F%A5)
- [string类型方法：index](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#string%E7%B1%BB%E5%9E%8B%E6%96%B9%E6%B3%95index)
- [string类型方法：substr](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#string%E7%B1%BB%E5%9E%8B%E6%96%B9%E6%B3%95substr)
- ["超级"or(条件联结)](https://github.com/hwding/perl6-doc-cn/blob/master/CH01.md#%E8%B6%85%E7%BA%A7or%E6%9D%A1%E4%BB%B6%E8%81%94%E7%BB%93)
### 第二章 元运算符
- What are the meta operators
- Assignment Operators
- Method invocation in assignment
- Calling a function during assignment
- Negated Relation Operators
- Reversed operators
- Hyper Operators
- Reduction operators
- Reduction Triangle operators
- Cross operators
### 第三章 Junctions in Perl6
- Junctions
- More tutorial with Junctions
### 第四章 Files in Perl6
- exit
- warn
- die
- Twigils and special variables
- Read line from file
- Read all the lines with get
- Process a file line by line
- Write to a file
- Open file modes
- slurp
- Read lines into array
- Exercise: Print sum of numbers
- Solution: Print sum of numbers
### 第五章 Perl6 Lists and Arrays
- List Literals, list ranges
- List Assignment
- Swap two values
- Loop over elements of list with for
- Create array, go over elements
- Array elements (create menu)
- Array assignment
- Command line options
- Process CSV file
- join
- The uniq functions
- Looping over a list of values one at a time, two at a time and more
- Looping over any number of elements
- Missing values
- Iterating over more than one array in parallel
- Z as in zip
- xx - string multiplicator
- sort values
- Transform arrays and lists using map
### 第六章 Perl6 Hashes
- Hashes (Associative Arrays)
- Fetching data from a hash
- Multidimensional hashes
- Count words
- Overview of hashes
- slurp hash
- kv
- Looping over keys of a hash
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
