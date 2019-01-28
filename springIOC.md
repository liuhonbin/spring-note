# springIOC

### what is IOC

``` 控制反转（Inversion of Control，缩写为IoC），是面向对象编程中的一种设计原则，可以用来减低计算机代码之间的耦合度。其中最常见的方式叫做依赖注入（Dependency Injection，简称DI），还有一种方式叫“依赖查找”（Dependency Lookup）```

### Dependency Injection

- 依赖注入

  1. 关于什么是依赖

  2. 关于注入和查找以及拖拽

     

### 为什么要使用spring IOC

spring体系结构----IOC的位置  自己看官网

1. 在日常程序开发过程当中，我们推荐面向抽象编程，面向抽象编程会产生类的依赖，当然如果你够强大可以自己写一个管理的容器，但是既然spring以及实现了，并且spring如此优秀，我们仅仅需要学习spring框架便可。
2. 当我们有了一个管理对象的容器之后，类的产生过程也交给了容器，至于我们自己的app则可以不需要去关系这些对象的产生了。

### spring实现IOC的思路和方法

1. spring实现IOC的思路是提供一些配置信息用来描述类之间的依赖关系，然后由容器去解析这些配置信息，继而维护好对象之间的依赖关系，前提是对象之间的依赖关系必须在类中定义好，比如A.class中有一个B.class的属性，那么我们可以理解为A依赖了B。既然我们在类中已经定义了他们之间的依赖关系那么为什么还需要在配置文件中去描述和定义呢？

   

   * spring实现IOC的思路大致可以拆分成3点

     1. 应用程序中提供类，提供依赖关系（属性或者构造方法

     2. 把需要交给容器管理的对象通过配置信息告诉容器（xml、annotation，javaconfig）

     3. 把各个类之间的依赖关系通过配置信息告诉容器

        

     ``1.配置这些信息的方法有三种分别是xml，annotation和javaconfig ``

     ``2.维护的过程称为自动注入，自动注入的方法有两种构造方法和setter ``

     ``3.自动注入的值可以是对象，数组，map，list和常量比如字符串整形等``

     

### spring编程的风格

1. schemal-based-------xml

2. annotation-based-----annotation

3. java-based----java Configuration

   

   







