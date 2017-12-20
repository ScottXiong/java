```
package com.imooc.oprater;

public class Sum {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
       //1到100累加
		/*int n=1, sum=0,m=1;
		while(n<101) {
			sum+=n;
			n++;
		}
		while(m<10000) {
			System.out.println("当前m为:"+m);
			m++;
		}
		System.out.println("1到100累加的结果为:"+sum);*/
		
		//1+3+5+..+99
		int n=1, sum=0;
		while(n<100) {
			sum+=n;
			n+=2;
		}
		System.out.println("1+3+5+..+99的和为："+sum);
	}

}

```
