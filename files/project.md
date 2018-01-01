# 工程，类，包
### 关系
工程用来装包的，包用来管理管理不同的类，一般会根据功能的不同而划分不同的包，包名以域名的倒叙命名（跨包访问需用import关键字eg`com.scott.school.*`）
- com.scott.school
- com.scott.test
### 类的创建
- 声明私有属性
- get/set方法
- 外加2个方法无参+有参构造（重载，方便初始化） 
- 打印信息
```
public String info(){
	String str="学生信息如下:\n学生姓名："+this.getStudentName()+"\n学号："+this.getStudentNo()+"\n年龄："+this.getStudentAge();
	return str;
}
```
