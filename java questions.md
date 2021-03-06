# Java 面试常考问答题
## Java basic 基础
- **== 和 equals 的区别是什么？**

  1.功能不同"=="是判断两个变量或实例是不是指向同一个内存空间。"equals"是判断两个变量或实例所指向的内存空间的值是不是相同。

  2.定义不同："equals"在JAVA中是一个方法。"=="在JAVA中只是一个运算符合。

  3.运行速度不同： "=="比"equals"运行速度快，因为"=="只是比较引用。 "equals"比"=="运行速度要慢。

- **final 在 java 中有什么作用？**

  当用final修饰一个类时，表明这个类不能被继承。

  当用final作用于类的成员变量时，成员变量（注意是类的成员变量，局部变量只需要保证在使用之前被初始化赋值即可）必须在定义时或者构造器中进行初始化赋值，而且final变量一旦被初始化赋值之后，就不能再被赋值了。

-	**java 中的 Math.round(-1.5) 等于多少？**
  
    Math.round采用的是+0.5，然后在进行向下取整，所以-1.5+0.5 = -1

- **继承和接口是什么？以及他们的区别**

  1.接口定义一个类需要实现的方法，属性，索引，时间和可能的参数，返回值类型，具体的实现交由相应的类或结构，从而使实现多态；而继承用在一个现有父类基础上的功能扩展，把及各类中间相同的成员提取出来，放在一个父类中，在子类中添加独特的方法，即继承扩展。

  2.接口能够实现多接口继承，而继承只能实现单继承。

  3.继承能都会得父类方法的实现，而接口只能获得方法的定义。

  4.在继承中，韦弗蕾添加方法不影响子类的继承，但接口中，为父类添加一个方法定义，必须在子类中添加此方法的实现。

-	**抽象类(abstract class)和接口(interface)的区别？**

    声明方法的类而不去实现它的类叫做抽象类，用 abstract 修饰，它用于要创建一个体现某些基本行为的类，并为该类声明方法，但却不实现。不能创建 abstract 类的实例，然而可以创建一个变量，其类型是一个抽象类，并让他指向具体子类的一个实例。不能由抽象构造函数或抽象静态方法。 Abstract 类的子类为他们父类中的所有抽象方法提供实现，否则他们也是抽象类。

    接口(Interface)是抽象类的变体，在接口中，所有方法都是抽象的。多继承性可以通过实现这样的接口而获得。接口中的方法都是抽象的，没有一个程序体，接口只可以定义 static final 成员变量。当类实现继承接口时，类中要定义实现所有接口的方法。

- **集合类都有哪几类？主要区别有哪些并简单描述？**

  集合类型主要有3种： set（集），list（列表）和 map（映射）

  set：
  1.它的对象不按特定方式排序，只是简单的把对象加入集合
  2.对集中的成员的访问和操作是通过集中对象的引用进行的，所及集中不能有重复对象。

  list：
  1.list接口与其实现类是容量可变的列表，可以按照索引访问集合中的元素，是有序的集合列表在数据结构分别表现为：数组和向量、链表、堆栈、队列。常用的有ArrayList。

  map:
  1.映射中每个项都是成对的，Map是把链对象和值对象进行关联的容器。2.
  映射中存储的每一个对象都有一个相关的关键字 key， 关键字决定了对象在映射中的存储位置，关键字应该是唯一的，常用的HashMap， TreeMap， HashTable。


  

