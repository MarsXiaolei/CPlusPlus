# C++程序设计<br>

[点我获取Github readme 编写语法规则]https://blog.csdn.net/guodongxiaren/article/details/23690801<br>

#### 前言

`程序追求的最高境界是:高内聚（函数功能越单一越好，目标越专一越好），低耦合（类与其他类关系越少越好）`<br>

`面向对象的三大特性：封装、继承、多态`。<br>

`读书需要多思考，特别是翻译的技术类书籍，需要多Google查证一下。`<br>

`读书从薄到厚，从厚到薄。`  <br>

`人的时间有限，需要多花点时间思考，该往哪个方向努力才能使利益最大化。`<br>

`无论什么时候都要保持清醒的头脑，明白自己想要什么，并为之奋斗。`<br>

[《C-Concurrency-in-Action-2nd-Edition》-C++并发编程英文版PDF](https://www.programmer-books.com/wp-content/uploads/2019/03/C-Concurrency-in-Action-2nd-Edition.pdf)<br>

#### 参考资料<br>
* 《华为C++代码规范》<br>
* 《C++高级编程》<br>
* 《传智播客轻松搞定 C++》<br>
* 《C++编程规范101条规则、准则与最佳实践》<br>
* 《深入应用C++ 11代码优化与工程级应用》<br>
* 《C++ Primer Plus》<br>
* 《深入理解计算机系统》<br>
* 《C++数据结构与算法》<br>
* 《传智播客轻松搞定设计模式》<br>
* 《C++并发编程实战第二版》<br>
* 《C++标准模板库编程实战》<br>

#### 设计模式
https://www.cnblogs.com/ring1992/p/9592428.html<br>
`下面为英文版本`<br>
https://github.com/JakubVojvoda/design-patterns-cpp<br>

#### 代码容器
![](https://github.com/MarsXiaolei/CPlusPlus/blob/master/%E6%89%B9%E6%B3%A8%202020-05-15%20141530.png)<br>

#### 进制转换<br>
[二、八、十、十六进制转换（图解篇）](https://www.cnblogs.com/gaizai/p/4233780.html)<br>

#### C++编译过程是怎样的？<br>

#### 内存管理
`在C++中，内存分成5个区，他们分别是堆、栈、自由存储区、全局/静态存储区和常量存储区。`<br>
https://chenqx.github.io/2014/09/25/Cpp-Memory-Management/<br>

#### 为什么要使用const常量取代宏？<br>
`宏是简单的文本替换，在预处理阶段时完成，运行报错时直接报相应的值；跟踪调试时也是显示值，而不是宏名；宏没有类型检查，不安全；宏没有作用域。`<br>
`示例：`<br>
`#define MAX_MSISDN_LEN (20) //不好的例子`<br>
`const int MAX_MSISDN_LEN = 20; //好的例子`<br>

#### C++作用域是什么？<br>
https://zh.cppreference.com/w/cpp/language/scope<br>

#### namespace命名空间使用<br>
`1、用途：解决命名冲突。`<br>
`2、命名空间下可以存放（变量、函数、结构体、类等）。`<br>
`3、命名空间只能存放在全局作用域下。`<br>
`4、命名空间可以嵌套命名空间。`<br>
`5、命名空间是开放的，可以随时添加新成员。`<br>
`6、命名空间可以是匿名的。`<br>
`7、命名空间可以起别名。`<br>

1、结构体和类的区别？<br>
2、两种单次编译方式的区别？<br>
3、const和宏的区别。<br>
4、函数参数按值、按指针、按引用、按const 引用传递的区别？<br>

#### 如何使用函数指针？<br>

#### 什么是回调函数，优缺点是什么？<br>


#### 什么时候使用类前置声明？<br>
`class A;`

#### C++类与类之间关系<br>
`依赖、关联、聚合、组合、继承、泛化`<br>
[]https://cloud.tencent.com/developer/article/1176331

#### C++构造函数初始化顺序
[构造函数]https://blog.csdn.net/qq_30835655/article/details/66971183

#### C++中类的内存布局
https://www.cnblogs.com/jiaochen/p/5524335.html

#### C++this指针详解
[this 指针]http://c.biancheng.net/cpp/biancheng/view/201.html

#### 为什么需要重载运算符？<br>

#### 如何正确使用访问标识符private、public、protected？<br>
`(1)需要被外界访问的成员直接设置为public。`<br>
`(2)只能在当前类中访问的成员设置为private。`<br>
`(3)只能在当前类和子类中访问的成员设置为protected，protected成员的访问权限介于public和private之间。`<br>
![](https://github.com/MarsXiaolei/CPlusPlus/blob/master/%E6%89%B9%E6%B3%A8%202020-05-14%20113253.png)

`多态是设计模式的基础，多态就是能够根据不同的对象而调用不同的接口。`<br>
[详细总结]https://blog.csdn.net/qq_39755395/article/details/79751362

#### 多态成立的条件是什么？<br>
`（1）要有继承。`<br>
`（2）要有虚函数重写。`<br>
`（3）父类指针指向子类对象。`<br>

#### 5、如何区分类中的重载(overload)、重写(Override覆盖)、隐藏(hide)？<br>
`相同点：就是大家的名称相同。`<br>
`重载是在同一个类中，而重写和隐藏是在基类和派生类中，这个很好区分，重点是区分重写和隐藏。`<br>
`（1）参数相同，如果基类函数有virtual，则为重写；如果基类函数无virtual，则为隐藏。`<br>
`（2）参数不同，不管有无virtual，都为隐藏。`<br>
`或者这样区分，更好理解，重写必须有virtual,且参数相同；参数不同和无virtual的都是隐藏。`<br>
`（1）基类函数有virtual，如果参数相同，则为重写；如果参数不同，则为隐藏。`<br>
`（2）基类函数无virtual，不管参数相不相同，都为隐藏。`<br>
[详细总结](https://blog.csdn.net/jixingzhong/article/details/1858943)<br>

#### 为什么要用多态？<br>
`多态有代码重用的功能，还可以解决项目中紧耦合的问题，提高程序的可扩展性。`<br>

#### 什么时候使用多态？<br>
`在设计模式中会用到多态，通常以下面两种方式出现：`<br>
`(1)父类指针作为函数的参数，将创建的子类对象作为实参传递。`<br>
`(2)父类指针作为函数的返回值，返回创建的子类对象。`<br>
[参考资料]https://blog.csdn.net/Ellen5203/article/details/87342706

#### 虚函数实现原理是什么？<br>
`虚函数表和vptr指针`<br>
https://blog.csdn.net/lihao21/article/details/50688337

#### 虚析构函数<br>
delete 基类指针时，会根据实际对象，调用相应的析构函数。
https://www.cnblogs.com/chio/archive/2007/09/10/888260.html

#### 什么是纯虚函数和抽象类？<br>
`纯虚函数没有函数体，只有函数声明，在虚函数声明的结尾加上=0，表明此函数为纯虚函数，无法调用，也无法为其分配内存空间。语法格式：`<br>
`virtual 返回值类型 函数名 (函数参数) = 0;`<br>
`包含纯虚函数（至少一个）的类称为抽象类（Abstract Class），抽象类无法实例化（创建对象）。`<br>
`抽象类通常是作为基类，让派生类去实现纯虚函数，派生类必须实现纯虚函数才能被实例化。`<br>

#### 标准模板库(STL)
`主要：`<br>
`(1)用于存储信息的容器；`<br>
`(2)用于访问容器存储的信息的迭代器；`<br>
`(3)用于操作容器内容的算法；`<br>

#### STL容器如何分类？
`容器分为顺序容器和关联容器。`<br>
`（1）顺序容器`<br>
`vector：操作与动态数组一样，在最后插入数据；可将 vector 视为书架，您可在一端添加和拿走图书。`<br>
`deque：与 vector 类似，但允许在开头插入或删除元素。`<br>
`list：操作与双向链表一样。可将它视为链条，对象被连接在一起，您可在任何位置添加或删除对象。`<br>
`forward_list：类似于 list，但是单向链表，只能沿一个方向遍历。`<br>
`（2）关联容器`<br>
`set：存储各不相同的值，在插入时进行排序；容器的复杂度为对数。`<br>
`unordered_set：存储各不相同的值，在插入时进行排序；容器的复杂度为常数。这种容器是 C++11 新增的。`<br>
`map：存储键-值对，并根据唯一的键排序；容器的复杂度为对数。`<br>
`unordered_map：存储键-值对，并根据唯一的键排序；容器的复杂度为对数。这种容器是C++11 新增的。`<br>
`multiset：与 set 类似，但允许存储多个值相同的项，即值不需要是唯一的。`<br>
`unordered_multiset：与 unordered_set 类似，但允许存储多个值相同的项，即值不需要是唯一的。这种容器是 C++11 新增的。`<br>
`multimap：与 map 类似，但不要求键是唯一的。`<br>
`unordered_multimap：与 unordered_map 类似，但不要求键是唯一的。这种容器是C++11新增的。`<br>
`(3)容器适配器`<br>
`容器适配器（Container Adapter）是顺序容器和关联容器的变种，其功能有限，用于满足特定的需求。`<br>
`stack：以 LIFO（后进先出）的方式存储元素，让您能够在栈顶插入（压入）和删除（弹出）元素。`<br>
`queue：以 FIFO（先进先出）的方式存储元素，让您能够删除最先插入的元素。`<br>
`priority_queue：以特定顺序存储元素，因为优先级最高的元素总是位于队列开头。`<br>
[参考资料]https://www.jianshu.com/p/497843e403b4

#### 如何使用C++多线程？
并发：两个或多个活动同时发生。

#### 如何使用C++

#### 字符串和字符格式转换

6、什么时候使用内联函数，有什么优缺点？<br>
8、使用智能指针的好处是什么？<br>
9、bool和BOOL的区别？<br>
10、函数默认参数怎么使用？<br>
11、派生类的访问权限是什么？<br>
12、什么是封装、继承、多态，有什么好处？<br>

14、为什么要重载运算符？<br>
15、如何使用条件编译？<br>
16、如何使用名称空间？<br>




