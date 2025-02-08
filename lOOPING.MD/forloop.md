## 61.Print numbers from 1 to 10 using for loop. 
````java[]

public class Main
{
	public static void main(String[] args) {
		for(int i=1;i<=10;i++){
		    System.out.print(i+" ");
		}
	}
}

OUTPUT:

1 2 3 4 5 6 7 8 9 10
````
## 62.Print the multiplication table of a number using for loop. 

````java[]



````

## 63.Calculate the factorial of a number using a for loop.

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the value of n");
	    int n=s.nextInt();
	    int fact=1;
		for(int i=1;i<=n;i++){
		   fact=fact*i;
		}
		System.out.println("factorial of "+n+"is :"+fact);
	}
}

OUTPUT:
Enter the value of n
7
factorial of 7is :5040


````

##  64.Print Fibonacci series up to n terms using for loop. 

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the value of n");
	    int n=s.nextInt();
	    int a=0;
	    int b=1;
	    System.out.println("fibonacci of "+n+" is :");
	    System.out.print(a+" "+b+" ");
		for(int i=1;i<=n;i++){
		  int c=a+b;
		  a=b;
		  b=c;
		
		System.out.print(c+" ");
	}
	}
}


OUTPUT:

Enter the value of n
8
fibonacci of 8is :
0 1 1 2 3 5 8 13 21 34
````
## 65.Sum of digits of a number using a for loop. 

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the value of n");
	    int n=s.nextInt();
	    int sum=0;
		for(int i=n;i>0;i/=10){
		    int a=i%10;
		    sum+=a;
		}
		System.out.print("sum of the digit "+n+" is: "+sum);
	}
	}


output:
Enter the value of n
89736
sum of the digit 89736 is: 33
````

##  66.Print prime numbers up to a given number using for loop. 

````java[]

`````

## 67.Reverse a number using for loop. 

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the value of n");
	    int n=s.nextInt();
	    int b=0;
		for(int i=n;i>0;i/=10){
		    int a=i%10;
		    b=b*10+a;
		}
		System.out.print("Reverse a digit "+n+" is: "+b);
	}
	}


OUTPUT:

Enter the value of n
86427
Reverse a digit 86427 is: 72468

````

## 68.Check whether a number is prime or not using a for loop. 

````java[]


````

## 69.Calculate the sum of even numbers from 1 to n using a for loop. 

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the value of n");
	    int n=s.nextInt();
	    int sum=0;
	    for(int i=0;i<=n;i++){
	        if(i%2==0){
	            sum+=i;
	        }
	    }
	    System.out.println("Sum of the even number from 1 to "+n+":"+sum);
	}
	}


OUTPUT:
Enter the value of n
20
Sum of the even number from 1 to 20:110

````

## 70.Calculate the sum of odd numbers from 1 to n using a for loop. 

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the value of n");
	    int n=s.nextInt();
	    int sum=0;
	    for(int i=0;i<=n;i++){
	        if(i%2!=0){
	            sum+=i;
	        }
	    }
	    System.out.println("Sum of the odd number from 1 to "+n+":"+sum);
	}
	}


OUTPUT:

Enter the value of n
30
Sum of the odd number from 1 to 30:225


````

