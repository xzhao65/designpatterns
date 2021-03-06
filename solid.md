### SOLID 原则

##### 1. Single Responsibility Principle 单一职责原则
##### 2. Open/closed Principle  开闭原则       
    对于扩展， 类应该是“开放”的； 对于修改， 类则应是“封闭”的。你可以创建一个子类并重写原始类的部分内容以完成不同的行为，而不是直接对原始类的代码进行修改。这样你既可以达成自己的目标，但同时又无需修改已有的原始类客户端。
##### 3.Liskov Substitution Principle  里氏替换原则
    当你扩展一个类时， 记住你应该要能在不修改客户端代码的情况下将子类的对象作为父类对象进行传递。
  * 子类方法的参数类型必须与其超类的参数类型相匹配或更加抽象
  * 子类方法的返回值类型必须与超类方法的返回值类型或是其子类别相匹配
  * 子类中的方法不应抛出基础方法预期之外的异常类型。
  * 子类不应该加强其前置条件。
  * 子类不能削弱其后置条件。
  * 超类的不变量必须保留。
  * 子类不能修改超类中私有成员变量的值。
##### 4.Interface Segregation Principle 接口隔离原则
    客户端不应被强迫依赖于其不使用的方法,你可将其拆分为更精细的接口，如有需要可在单个类中实现所有接口，某些类也可只实现其中的一个接口。
##### 5.Dependency Inversion Principle 依赖倒置原则
    高层次的类不应该依赖于低层次的类。两者都应该依赖于抽象接口。抽象接口不应依赖于具体实现。具体实现应该依赖于抽象接口。
  
    依赖倒置原则通常和开闭原则共同发挥作用：你无需修改已有类就能用不同的业务逻辑类扩展低层次的类。
  ![image](https://user-images.githubusercontent.com/33577671/119323905-c7aa6b80-bcb1-11eb-955e-a398db59c5d8.png)
  ![image](https://user-images.githubusercontent.com/33577671/119324391-57e8b080-bcb2-11eb-8912-aa76c012a04c.png)

