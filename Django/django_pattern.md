# 什么是MVC模式

MVC全名是Model View Controller，是模型(model)－视图(view)－控制器(controller)的缩写，一种软件设计典范，用一种业务逻辑、数据、界面显示分离的方法组织

代码，将业务逻辑聚集到一个部件里面，在改进和个性化定制界面及用户交互的同时，不需要重新编写业务逻辑。MVC被独特的发展起来用于映射传统的输入、处理和输出功

能在一个逻辑的图形化用户界面的结构中。 通俗的来讲就是，强制性的使应用程序的输入，处理和输出分开。

###### 核心思想：解耦
优点：减低各个模块之间的耦合性，方便变更，更容易重构代码，最大程度的实现了代码的重用

MVC(Model, View, Controller) Model: 即数据存取层。用于封装于应用程序的业务逻辑相关的数据，以及对数据的处理。说白了就是模型对象负责在数据库中存取数据

View: 即表现层。负责数据的显示和呈现。渲染的html页面给用户，或者返回数据给用户。

Controller: 即业务逻辑层。负责从用户端收集用户的输入，进行业务逻辑处理，包括向模型中发送数据，进行CRUD操作



# 什么是MVT模式

严格来说，Django的模式应该是MVT模式，本质上和MVC没什么区别，也是各组件之间为了保持松耦合关系，只是定义上有些许不同。

Model： 负责业务与数据库(ORM)的对象

View： 负责业务逻辑并适当调用Model和Template

Template: 负责把页面渲染展示给用户

注意： Django中还有一个url分发器，也叫作路由。主要用于将url请求发送给不同的View处理，View在进行相关的业务逻辑处理
