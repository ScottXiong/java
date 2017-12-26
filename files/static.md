# static
static的主要作用就是共享数据，遇到一个类的多个对象共享数据的地方都可以使用static。在后面的课程中会多次用到static，比如和final一起使用 ，以及单例模式中，单例模式也可以算作static的一个应用。
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
