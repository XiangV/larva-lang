larva-lang
==========

原转为java的项目版本已迁移至个人，请访问：

<https://github.com/maopao-691515082/larva-lang_4j>

简介：

一个用go做后端的语言

特点：

1 语法贴近C++、Java、C#这一系列，吸收了Go中个人认为较好的一些设计，静态类型，编译到Go语言代码，后端利用Go的工具和环境

2 对Go语言语法较为晦涩或不太符合习惯的地方做了修改，例如类型系统采用Java和C#的方式（对象用引用传递）；将Go的匿名包含改成了类似的usemethod机制；一定程度上允许循环import；等等

3 除语法的区别外，对Go语言的一些不足之处做了补充，例如支持泛型类和泛型函数，且实现方式为编译期展开（类似C++模板的处理），基本无性能损耗

4 Larva源代码和Go语言目标代码的对应规则简单明了，用Go开发native模块很方便，但是标准库和运行时对Go语言的native实现依赖降低，大量lib将采用Larva自身实现

大体进度和TODO：

1 语法基本完成，编译器和runtime的剩余工作就是测试和修复bug

2 还需补充必要的基础库，包括os、net等库，以及Vector之类的泛型类库

3 补充文档

近期计划：

1 interface的继承语法

2 for (iter: \[iterator | iterable\])语法

3 完整的反射实现

生了二胎，最近没空搞了。。。
