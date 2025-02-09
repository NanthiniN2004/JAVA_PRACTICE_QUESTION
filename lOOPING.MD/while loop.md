## 81.Print numbers from 1 to 10 using while loop. 

````java[]

public class Main
{
	public static void main(String[] args) {
	    int i=1;
		while(i<=10){
		    System.out.print(i+" ");
		    i++;
		}
	}
}

OUTPUT:

1 2 3 4 5 6 7 8 9 10 


````

## 82.Print all even numbers up to n using while loop. 

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the value of n");
	    int n=s.nextInt();
	    int i=1;
	    System.out.println("Even numbers");
		while(i<=n){
		   if(i%2==0){
		       System.out.print(i+" ");
		   }
		   i++;
		}
	}
}

OUTPUT:

Enter the value of n
25
Even numbers
2 4 6 8 10 12 14 16 18 20 22 24 

````

## 83.Calculate the factorial of a number using while loop. 

````java[]
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the value of n");
	    int n=s.nextInt();
	    int fact=1;
	    int i=1;
		while(i<=n){
		   fact=fact*i;
		   i++;
		}
		System.out.println("factorial of "+n+"is :"+fact);
	}
}

OUTPUT:

Enter the value of n
5
factorial of 5is :120

````


## 84.Reverse a number using while loop. 

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the value of n");
	    int n=s.nextInt();
	    int b=0;
		while(n!=0){
		    int a=n%10;
		    b=b*10+a;
		    n/=10;
		}
		System.out.print("Reverse a digit "+n+" is: "+b);
	}
	}
OUTPUT:

Enter the value of n
79264
Reverse a digit 79264 is: 46297

````

## 85.Print Fibonacci series up to n terms using while loop. 
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
	    int i=1;
		while(i<=n){
		  int c=a+b;
		  a=b;
		  b=c;
		
		System.out.print(c+" ");
		i++;
	}
	}
}

Enter the value of n
10
fibonacci of 10 is :
0 1 1 2 3 5 8 13 21 34 55 89 
````


## 86.Sum of digits of a number using while loop. 
````java[]


import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the value of n");
	    int n=s.nextInt();
	    int sum=0;
		while(n!=0){
		    int a=n%10;
		    sum+=a;
		    n/=10;
		}
		System.out.print("sum of the digit "+n+" is: "+sum);
	}
	}

output:

Enter the value of n
936814
sum of the digit 936814 is: 31

````

## 87.Print all odd numbers up to n using while loop. 

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the value of n");
	    int n=s.nextInt();
	    int i=1;
	    System.out.println("Even numbers");
		while(i<=n){
		   if(i%2!=0){
		       System.out.print(i+" ");
		   }
		   i++;
		}
	}
}

output:

Enter the value of n
30
Even numbers
1 3 5 7 9 11 13 15 17 19 21 23 25 27 29 

````
## 88.Find the sum of natural numbers using while loop. 

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
		Scanner s=new Scanner(System.in);
		System.out.println("Enter the value of n");
		int n=s.nextInt();
		int sum=0;
		int i=0;

		while(i<=n) {
			sum+=i;
			i++;
		}
 System.out.println("Sum of first " + n + " natural numbers is: " + sum);

	}
}


OUTPUT:

Enter the value of n
5
Sum of first 5 natural numbers is: 15


````
## 89.Count the number of digits in a number using while loop. 

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the value of n");
	    int n=s.nextInt();
	    int count=0;
		while(n!=0){
		    int a=n%10;
		    count++;
		    n/=10;
		}
		System.out.print("count of the digit "+n+" is: "+count);
	}
	}

OUTPUT:

Enter the value of n
6928394
count of the digit 6928394  is: 7

````

## 90.Calculate the product of digits of a number using while loop. 

````java[]
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the value of n");
	    int n=s.nextInt();
	    int prod=1;
		while(n!=0){
		    int a=n%10;
		    prod*=a;
		    n/=10;
		}
		System.out.print("Product of the digit "+n+" is: "+prod);
	}
	}

OUTPUT:
Enter the value of n
873
Product of the digit 873 is: 168


````
