### 解决作用域的2个方案
- 将i声明在外面，扩大它的生命周期(当方法的返回值为空时，return可以直接结束方法，break是结束循环)
```
for(int i=0;i<this.getMystudents().length;i++) {
	if(this.getMystudents[i]==null)
		this.studentsNo=i+1;
		break;
}
```
```
int i;
for( i=0初始化;i<this.getMystudents.length;i++) {
	if(this.getMystudents()[i]==null)
		return;
}
this.studentsNo=i+1;
```
