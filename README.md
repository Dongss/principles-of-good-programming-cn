# 优秀的编程原则

[翻译自: Principles of Good Programming](https://www.artima.com/weblogs/viewpost.jsp?thread=331531)

### DRY - Don’t repeat yourself

**不要重复自己**

这大概是编程最基本的原则。也由此产生了很多编程的概念（比如循环，函数，类，等等）。一旦我们开始重复自己，就应该考虑做一下抽象了。

https://en.wikipedia.org/wiki/Don%27t_repeat_yourself

### Abstraction Principle

**抽象原则**

抽象原则也和 DRY 原则有关，“程序中的每段核心功能代码应该只在源代码中的一个地方实现”。

http://en.wikipedia.org/wiki/Abstraction_principle_(programming)

### KISS (Keep it simple, stupid!)

**代码简洁**

代码简洁是一个很重要的目标，写简洁的代码耗费的时间更少、bug 更少、更易于修改。

http://en.wikipedia.org/wiki/KISS_principle

### Avoid Creating a YAGNI (You aren’t going to need it)

如果某个功能你还用不到，就不要去实现它。

http://en.wikipedia.org/wiki/YAGNI

### Do the simplest thing that could possibly work

**用最简单的方式解决问题**

时常问自己“能解决问题（完成需求）的最简单的方式是什么？”，有利于设计方案的简洁明了。

http://c2.com/xp/DoTheSimplestThingThatCouldPossiblyWork.html

### Don’t make me think

**不要让我思考**

这正是 Steve Krug 的一本关于 web 可用性的书的标题，同样适用于编程。代码应该保持简洁易读，如果读起来太过复杂，应该简化一下。

http://www.sensible.com/dmmt.html

### Open/Closed Principle

**开闭原则**

软件功能（类，模块，函数等等）应对拓展开放，对修改封闭。换句话说，不要写需要别人修改的类，要写便于别人拓展的类。

http://en.wikipedia.org/wiki/Open_Closed_Principle

### Write Code for the Maintainer

**写易维护的代码**

几乎所有代码都是需要长期维护的，不管是你自己维护还是别人维护。即使是自己的代码，一段时间以后自己也可能忘记里面的逻辑，所以相当于写代码的人和维护的人不是同一个。有这么个方法“写代码的时候记着，将来维护代码的人是一个知道你住在哪里的变态暴力狂”。

http://c2.com/cgi/wiki?CodeForTheMaintainer


### Principle of least astonishment

**减少误导**

这个原则通常在接口上被提到，但在代码里也很重要，代码不应该误导阅读者。注释的说明要和代码一致，函数名要和函数内容一致，要避免迷惑和误导。

http://en.wikipedia.org/wiki/Principle_of_least_astonishment

### Single Responsibility Principle

**单一功能原则**

一段代码（类或函数）应只实现一个单一的定义清晰的任务。

http://en.wikipedia.org/wiki/Single_responsibility_principle

### Minimize Coupling

**低耦合**

代码的任何部分（代码块，函数，类等等）都应该减少对其他部分代码的依赖，要尽量减少变量共享。“低耦合通常是结构优秀的计算机系统和好的设计的标志，配合高内聚，就能实现高可读和易维护的目标”。

http://en.wikipedia.org/wiki/Coupling_(computer_programming)

### Maximize Cohesion

**高内聚**

实现一个功能相关的代码，都应在同一个模块中实现。

http://en.wikipedia.org/wiki/Cohesion_(computer_science)

### Hide Implementation Details

**隐藏实现细节**

隐藏实现细节，当内部逻辑修改时，能够减少对其他使用者的影响。

http://en.wikipedia.org/wiki/Information_Hiding

### Law of Demeter

**迪米特法则**

代码应该跟有直接关联的部分交互（比如类继承的父类、包含的对象、传入的参数，等等）。

http://en.wikipedia.org/wiki/Law_of_Demeter

### Avoid Premature Optimization

**避免过早优化**

代码还在正常工作的时候不必考虑优化，除非运行速度不及预期，并且最好在有量化数据对比的前提下进行。“我们应忽略小的影响，大约97%的情况下：过早优化是万恶之源” -- Donald Knuth。

http://en.wikipedia.org/wiki/Program_optimization

### Code Reuse is Good

**代码复用**

代码复用可以提高代码可用性并减少开发时间。

http://en.wikipedia.org/wiki/Code_reuse

### Separation of Concerns

**关注分离**

不同的功能应分开管理并有明显界限，要最大程度降低模块间代码的重叠。

http://en.wikipedia.org/wiki/Separation_of_concerns

### Embrace Change

**拥抱变化**

这是 Kent Beck 一本书的子题目，也是极限编程和敏捷开发的一个宗旨。很多其他的原则都是基于期望并拥抱变化的初心，一些传统的软件工程原则比如“低耦合”都有利于更简单的修改代码。不管你是不是极限编程爱好者，这个原则对写代码都很有帮助。

http://www.amazon.com/gp/product/0321278658