### 解决作用域的2个方案
- 将i声明在外面，扩大它的生命周期
```
for(int i=0;i<this.getMystudents.length;i++) {
	if(this.getMystudents[i]==null)
		studentsNo=i;
		break;
}
```
```
i=0;
for( i=0;i<this.getMystudents.length;i++) {
	if(this.getMystudents[i]==null)
		continue;
}
studentsNo=i;
```
