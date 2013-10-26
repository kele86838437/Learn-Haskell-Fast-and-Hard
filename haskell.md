快速穿越Haskell荆棘
====================
![github](imag/magritte_pleasure_principle.jpg "Title")

一篇短而不失技术含量的Haskell教程。

目录
----

*	[引言](#引言)
*	[致谢](#致谢)

我认为所有的开发者都应该去学习一下Haskell。虽然没有必要成为Haskell方面的大牛，但是了解Haskell所<br>
支持的特性能够开阔你的视野。

主流的语言通常都有一些共同特点：

-变量 <br>
-循环 <br>
-指针[<sup>1</sup>](#致谢) <br>
-数据结构，对象和类（更多...） <br>

Haskell非常独特。这门语言使用的很多概念是我之前从未接触过的。而这些编程思想能够使你成为优秀的程序员。

对我来，说学习Haskell确实有难度。在文章中，我会把我学习过程中遇见的困惑呈现出来，以便大家提高。

学习Haskell没有捷径可走，正是这样，这篇文章理解起来还是存在难度的。Haskell的掌握带有难度和挑战，我 <br>
认为这是一件好事。由于Haskell不容易理解，学习起来才充满意义。

通常学习Haskell方法是去学习两本经典的书，一本是[Learn You a Haskell](http://learnyouahaskell.com/),另一本则是[Real World Haskell](http://www.amazon.cn/dp/0596514980) 。<br>
我非常赞同，如果想你全面掌握Haskell，精读这两部著作是必不可少的。

然而，这篇文章非常简单的囊括了Haskell所带有的主要特点。同时文中也会包涵我在学习Haskell的疑惑之处。

文章内容分成五部分：

*	引言：一些简短的例子展示Haskell人性化之处
*	Haskell基础：Haskell语法以及一些重要的概念
*	困难部分：
	*	函数式风格；包含一个更深入的例子，展示了从命令式到函数式风格的转变
	*	类型；包含类型和标准二叉书的例子
	*	无限结构体；包含修改一棵无限的二叉树的例子！
*	超级困难部分：
	*	IO 处理；包含一个短小的例子
	*	IO 技巧展示；由于我对IO了不够了解，其中没有涉及具体的IO细节
	*	单体；难以置信的运行结果；
*	附录：
	*	更多关于无限树的知识；从数学方面来讨论无限树的概念

				提示：当看到一个文件名以.lhs后缀结尾，你可以单击单击文件名然后取得该文件。如果你将该文件另存为
				filename.lhs，可以通过如下命令运行
					runhaskell filename.lhs	
				除了一小部分外，大部分源码文件能够正常运行。
	
[00_hello_world.lhs](code/00_hello_world.lhs)
###1.引言###
####1.1安装####
![github](imag/Haskell-logo.png)

[Haskell Platform](http://www.haskell.org/platform/)上提供各平台上的Haskell安装方式。

工具：

-ghc：编译器类似于C语言的编译器gcc。<br>
-ghci：Haskell的控制台交互程序 (REPL)<br>
-runhaskell：用于直接运行一个事先没有编译的程序，这样虽然比较方便但比起先编译好在运行的要慢得多<br>

####1.2莫要惊慌####
![github](imag/munch_TheScream.jpg)

许多介绍Haskell的书或文章通常会以引入深奥的公式开篇(如快排，斐波那契等公式)。
###致谢###
1.尽管大多数现代编程语言尽力去规避它，但是它还是会以另一种形式表示出来。
