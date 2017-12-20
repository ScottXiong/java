```
package com.imooc.oprater;

import java.util.Scanner;

public class ConditionDemo2 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		System.out.print("请输入一个整数");
    Scanner s=new Scanner(System.in);
    int num= s.nextInt();
    if(num%2==0) {
    	 System.out.print(num+"是偶数");
    }else {
    	 System.out.print(num+"是奇数");
    }
	}

}

```
