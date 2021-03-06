##Introduction 
####介绍
The JavaScript core language features are defined in a standard called ECMA-262. The language defined in this standard is called ECMAScript, of which the JavaScript in the browser and Node.js environments are a superset. While browsers and Node.js may add more capabilities through additional objects and methods, the core of the language remains as defined in ECMAScript, which is why the ongoing development of ECMA-262 is vital to the success of JavaScript as a whole.

JavaScript核心特性根据 ECMA-262 标准制定。语言的核心特性在标准中被称为ECMAScript，并且是作为一个父集存在于浏览器和NodeJs环境中。当浏览器和NodeJs可通过额外的对象和方法来增加更多的功能，这种核心特性就会被定义为ECMAScript，这就是为什么ECMA-262标准的持续发展对JavaScript作为一个整体能否成功起着至关重要的作用。


In 2007, JavaScript was at a crossroads. The popularity of Ajax was ushering in a new age of dynamic web applications while JavaScript hadn’t changed since the third edition of ECMA-262 was published in 1999. TC-39, the committee responsible for driving the ECMAScript process, put together a large draft specification for ECMAScript 4. ECMAScript 4 was massive in scope, introducing changes both small and large to the language. Language features included new syntax, modules, classes, classical inheritance, private object members, optional type annotations, and more.

在2007年，JavaScript发展处于一个十字路口。Ajax的普及开创了一个新的动态的web应用程序时代，但JavaScript并没有更新因为ECMA-262的第3版是在1999年推出。负责ECMAScript的委员会TC-39为ECMAScript4起草了一个大规范。ECMAScript4是大规模的改变，更改了语言从小到大的部分，包括新的语法、模块、类、经典继承、私有对象成员、可选的类型注释、以及更多。


The scope of the ECMAScript 4 changes caused a rift to form in TC-39, with some members feeling that the fourth edition was trying to accomplish too much. A group of leaders from Yahoo, Google, and Microsoft came up with an alternate proposal for the next version of ECMAScript that they initially called ECMAScript 3.1. The “3.1” was intended to show that this was an incremental change to the existing standard.

ECMAScript4改变的部分引起了TC-39的内部形成了分裂，一些成员觉得第4版试图完成的部分太多了。来自Yahoo, Google, 和 Microsoft的领导完成了ECMAScript的下一个版本，该版本一开始被称为ECMAScript 3.1。3.1版本意图是对现有版本循循渐进的改变。


ECMAScript 3.1 introduced very few syntax changes, instead focusing on property attributes, native JSON support, and adding methods to already-existing objects. Although there was an early attempt to reconcile ECMAScript 3.1 and ECMAScript 4, this ultimately failed as the two camps had difficulty with the very different perspectives on how the language should grow.

ECMAScript 3.1介绍了非常少的语法变化，反而侧重于property属性，本地JSON支持和对已经存在的对象添加方法。尽管ECMAScript 3.1和 ECMAScript 4早期企图调和，但这终将失败，因为这两阵营对于语言的发展的视角非常不一样。


In 2008, Brendan Eich, the creator of JavaScript, announced that TC-39 would focus its efforts on standardizing ECMAScript 3.1. They would table the major syntax and feature changes of ECMAScript 4 until after the next version of ECMAScript was standardized, and all members of the committee would work to bring the best pieces of ECMAScript 3.1 and 4 together after that point into an effort initially nicknamed ECMAScript Harmony.

在2008年，JavaScript的创始人Brendan Eich宣布TC-39将致力于规范ECMAScript 3.1。他们将集中讨论ECMAScript 4主要变化的语法和特性直到ECMAScript下一个版本标准化，并且所有委员会的成员将努力汇集 ECMAScript 3.1 和 4 最佳的特性，在这之后这些特性会指向一个起初被叫作“ECMAScript Harmony”绰号的努力。


ECMAScript 3.1 was eventually standardized as the fifth edition of ECMA-262, also described as ECMAScript 5. The committee never released an ECMAScript 4 standard to avoid confusion with the now-defunct effort of the same name. Work then began on ECMAScript Harmony, with ECMAScript 6 being the first standard released in this new “harmonious” spirit.

ECMAScript 3.1最终被规范为ECMA-262的第5个版本，也就是ECMAScript 5。委员会没有把该版本以ECMAScript 4命名发布是为了避免和之前讨论的ECMAScript 4同名而造成混乱。然后工作开始于ECMAScript Harmony，ECMAScript 6成为这种新的“Harmony”精神的第一个标准。


ECMAScript 6 reached feature complete status in 2015 was formally dubbed “ECMAScript 2015” (though this text still refers to it as ECMAScript 6, the name most familiar to developers). The features vary widely from completely new objects and patterns to syntax changes to new methods on existing objects. The exciting thing about ECMAScript 6 is that all of these changes are geared towards problems that developers are actually facing. And while it will still take time for adoption and implementation to reach the point where ECMAScript 6 is the minimum that developers can expect, there’s a lot to be gained from a good understanding of what the future of JavaScript looks like.

ECMAScript 6在2015年达到功能完整的状态并被正式命名为ECMAScript 2015（但本文还是叫它为大多数开发者熟悉的ECMAScript 6）。The features vary widely from completely new objects and patterns to syntax changes to new methods on existing objects. 令人兴奋的是ECMAScript 6的所有这些变化是针对开发者所面临的问题。虽然对于采用和实施以达到让开发者所期望的ECMAScript 6的最基本内容还需要些时间，还有很多好的方式可以知道JavaScript的特性是怎样的。

##Browser and Node.js Compatibility 
####浏览器和NodeJs的兼容性
Many JavaScript environments, such as web browsers and Node.js, are actively working on implementing ECMAScript 6. This book does not attempt to address the inconsistencies between implementations and instead focuses on what the specification defines as the correct behavior. As such, it’s possible that your JavaScript environment may not conform to the behavior described in this book.

很多JavaScript环境，如浏览器和NodeJs,正在努力实现ECMAScript。这本书不是尝试划分实现间的不一致，取而代之的是把重点放在规范定义的正确行为上。因此，你的JavaScript环境可能不符合这本书讨论的行为。

##Who This Book is For 
####这本书适合谁看
This book is intended as a guide for those who are already familiar with JavaScript and ECMAScript 5. While a deep understanding of the language isn’t necessary to use this book, it is helpful in understanding the differences between ECMAScript 5 and 6. In particular, this book is aimed at intermediate-to-advanced JavaScript developers (both browser and Node.js environments) who want to learn about the future of the language.

这本书的目的是作为一个为那些已经熟悉JavaScript和ECMAScript 5开发者的指南。这本书不适合用来深入理解语言，它只是用来帮助理解ECMAScript 5 和 6之间的区别。特别是，这本书这本书是针对想要了解语言未来的中级到高级的JavaScript开发者（包括浏览器和Node.js环境）。

This book is not for beginners who have never written JavaScript. You will need to have a good basic understanding of the language to make use of this book.

这本书不适合没写过JavaScript的开发者。你需要一个不错的语言基础才能看懂本书的内容。


##Overview
####概述
Chapter 1: Block Bindings talks about let and const, the block-level replacement for var.

第1章：替换 var 的块级别绑定 let 和 const 。


Chapter 2: Strings and Regular Expressions covers the additions to string manipulation and inspection as well as the introduction of template strings.

第2章：字符串扩展，包括Strings、Regular Expressions 和模板字符串

Chapter 3: Functions discusses the various changes to functions. This includes the arrow function form, default parameters, rest parameters, and more.

第3章：讨论函数的各种变化，包括 arrow，默认参数，其他参数，以及更多。

Chapter 4: Objects explains the changes to how objects are created, modified, and used. Topics include changes to object literal syntax, and new reflection methods.

第4章：对象扩展解释了对象的创建、修改和使用的变化。主题还讨论对象字面量的语法和新的反射方法。


Chapter 5: Destructuring introduces object and array destructuring, which allow you to decompose objects and arrays using a concise syntax.

第5章：解构对象和数组。


Chapter 6: Symbols introduces the concept of symbols, a new way to define properties. Symbols are a new primitive type that can be used to obscure (but not hide) object properties and methods.

第6章：介绍新的原始数据类型Symbols，可以用来掩盖（但不隐藏）对象的属性和方法。

Chapter 7: Iterators and Generators discusses the addition of iterators and generators to the language. These features allow you to work with collections of data in powerful ways that were not possible in previous versions of JavaScript.

第7章：迭代器和生成器扩展允许收集通过强大的方式收集数据。


Chapter 8: Classes introduces the first formal concept of classes in JavaScript. Often a point of confusion for those coming from other languages, the addition of class syntax in JavaScript makes the language more approachable to others and more concise for enthusiasts.

第8章：类在JavaScript中第一次有正式概念。常常和其他语言的 class 造成混乱，JavaScript添加的 class 语法使开发者更容易使用。

Chapter 9: Arrays details the changes to native arrays and the interesting new ways they can be used in JavaScript.

第9章：数组详述了原生数组的改变和新的有趣的方法。

Chapter 10: Collections details the new collection types of Set, WeakSet, Map, and WeakMap. These types expand on the usefulness of arrays by adding semantics, de-duping, and memory management designed specifically for JavaScript.

第10章：新的收集方式 Set, WeakSet, Map 和 WeakMap，这些方式通过添加语义，de-duping和专门为JavaScript设计的内存管理以提高数组的效率。

Chapter 11: Promises introduces promises as a new part of the language. Promises were a grassroots effort that eventually took off and gained in popularity due to extensive library support. ECMAScript 6 formalizes promises and makes them available by default.

第11章：

Chapter 12: Reflection introduces the formalized reflection API for JavaScript. Similar to other languages, ECMAScript 6 reflection allows you to inspect objects at a granular level, even if you didn’t create the object.

第12章：介绍JavaScript正式的reflection API，允许检查对象的粒度级别，即使没有创建对象。

Chapter 13: Proxies discusses the new proxy object that allows you to intercept every operation performed on an object. Proxies give developers unprecedented control over objects and, as such, unlimited possibilities for defining new interaction patterns.

第13章：介绍新的代理对象，允许拦截对象上的每一个操作。代理给开发者提供了对对象前所未有的控制，因此，这种新的交互模式提供了无需的可能。


Chapter 14: Modules details the official module format for JavaScript. The intent is that these modules can replace the numerous ad-hoc module definition formats that have appeared over the years.

第14章：介绍模块的格式，这些模块可以取代已经出现了多年的众多的特设模块格式。

##Help and Support
You can file issues, suggest changes, and open pull requests against this book by visiting: https://github.com/nzakas/understandinges6

For anything else, please send a message to the mailing list: http://groups.google.com/group/zakasbooks.


