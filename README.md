# java
- [接口](https://github.com/ScottXiong/java/blob/master/files/interface.md)
- [键盘输入](https://github.com/ScottXiong/java/blob/master/files/tap.md)
### 注意
- switch case 结构一旦匹配到常量遇到break（如果不加break，一旦匹配到则会把后面的所有也执行掉）就跳出switch结构，如果一个都没匹配到也回自动跳出循环
- 嵌套：遇到大括号就保留2个空格的锁进，有的公司是四个
- while循环：1，初始化 2，控制循环条件-使n不断变化（否则就是死循环）
- 涉及到阶乘要用long定义
- 注意循环嵌套，需要第二次初始化1！+2！+3!+...+10!;直角三角形
- 要深刻理解为什么有变量和条件控制的概念
- static关键字：用static修饰的（实际上是操作的同一块内存空间）叫类成员，也叫静态成员，公用属性。无论实例化多少次，任何一个实例的改变都会改变，因为操作的同一块内存空间，所以此处的price会以最后一次赋值为准`public static int price`；å，类对象共享。ß，此外static修饰的变量很长寿，从类第一次加载时产生，到这个类彻底销毁才会进行资源释放;静态属性有2种访问方法：class.price obj1.price,即类名访问和实例化对象访问
- static 声明静态属性&静态方法，没用static修饰之前只是普通的成员，用static修饰之后就升官为类属性和方法了；当然，即然荣升为类了，最好用类名去访问（想访问外层的属性和方法可以用 类. obj. 还可以直接eat()）
```
public cat{
 this.eat();
 eat();
 this.name;
}
```
- static只能修饰最外层的属性和方法，这就意味着局部变量不能用static
```
public Cat(){
 static int price;//会报错
}
```
- 静态方法，只能访问静态属性和方法，直接访问一定会报错；除非把他们都设置成静态的，要么就在方法内部实例化一个对象，通过对象的形式去访问。
```
static void Cat(){
  Cat temp=new Cat();
  temp.name="xxx";
  temp.run();
}
```
- class只能用public abstract & final修饰；可以有静态属性和方法，但是绝对不会有静态的类

### fun
- string.toUpperCase()
