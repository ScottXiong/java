# 工程，类，包,成员属性
### 关系
工程用来装包的，包用来管理管理不同的类，一般会根据功能的不同而划分不同的包，包名以域名的倒叙命名（跨包访问需用import关键字eg`com.scott.school.*`）
- com.scott.school
- com.scott.test
### 类的创建
- 声明私有属性
- get/set方法：int类型添加逻辑判断
- 外加2个方法：无参+多参构造（重载，方便初始化） 
- 打印信息：字符串返回的方式更适合多平台的展示
```
public String info(){
	String str="学生信息如下:\n学生姓名："+this.getStudentName()+"\n学号："+this.getStudentNo()
	+"\n年龄："+this.getStudentAge();
	return str;
}
//想一想这里为什么没有用print语句打印？因为现在是控制台，如果换成了模拟器？浏览器？就不能正常输出了：你不需要打印，只需要
提供信息即可---提高了代码的复用性
```
### 成员属性特点
- get/set方法：如果成员属性是对象，在get方法之前，必要对其进行实例化，防止对象未初始化报错
- 无参/有参构造
- 必用this调用
