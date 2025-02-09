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

##  91.Find the greatest common divisor (GCD) using while loop.

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
		System.out.println("Enter the two value");
		int n1=s.nextInt();
		int n2=s.nextInt();
		while(n1!=n2){
            if(n1>n2){
                n1-=n2;
            }
            else{
                n2-=n1;
            }
        }
        System.out.println("Gcd of numbers "+n1);
	}
}


OUTPUT:

Enter the two value
20
30
Gcd of numbers 10

````

## 92. Reverse a string using while loop. 

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	System.out.println("Enter the String");
	String str=s.nextLine();
	String rev="";
	int n=str.length()-1;
	int i=n;
	while(i>=0){
	    rev+=str.charAt(i);
	    i--;
	}
	System.out.println(rev);
	}
}


OUTPUT:

Enter the String
Hello
olleH


````

## 93. Sum all odd numbers in a range using while loop.

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
         System.out.println("Enter the start value");
         int start=s.nextInt();
         System.out.println("Enter the end value");
         int end=s.nextInt();
         int sum=0;
         int i=start;
         while(i<=end){
             if(i%2!=0){
                 sum+=i;
             }
             i++;
         }
         System.out.println(" Sum all odd numbers in " +start+ " to " +end+ sum);
	}
}


OUTPUT:

Enter the start value
1
Enter the end value
25
Sum all odd numbers in 1 to 25 169

````

## 94.Print even numbers from a range using while loop. 

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
         System.out.println("Enter the start value");
         int start=s.nextInt();
         System.out.println("Enter the end value");
         int end=s.nextInt();
         int i=start;
         System.out.println("Even number");
         while(i<=end){
             if(i%2==0){
                 System.out.print(i+" ");
             }
             i++;
         }
	}
}


OUTPUT:

Enter the start value
2
Enter the end value
40
Even number
2 4 6 8 10 12 14 16 18 20 22 24 26 28 30 32 34 36 38 40

````

## 95.Find the sum of even and odd digits of a number. 

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
         System.out.println("Enter the start value");
         int n=s.nextInt();
         int sumodd=0;
         int sumeven=0;
         while(n!=0){
             int a=n%10;
             if(a%2!=0){
                 sumodd+=a;
             }
             else{
                 sumeven+=a;
             }
             n/=10;
         }
         System.out.println(" sum of the even digit "+sumeven);
         System.out.println(" sum of the odd digit "+ sumodd);
        
	}
}


OUTPUT:

Enter the start value
96246105
 sum of the even digit 18
 sum of the odd digit 15


````
## 96.Find the factorial of a number using while loop. 

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
         System.out.println("Enter the value");
         int n=s.nextInt();
         int i=1;
         int fact=1;
         while(i<=n){
            fact=fact*i;
             i++;
         }
         System.out.println(" Factorial of number "+fact);
         
        
	}
}


OUTPUT:

Enter the value
5
 Factorial of number 120

````
## 97.Find the largest prime number in a given range.
````JAVA[]

import java.util.*;
public class Main {
         public static boolean isprime(int num){
             if(num<2){
                 return false;
             }
            int i=2;
        while(i<=num/2){
        if(num%i==0){
            return false;
        }
        i++;
   } 
        return true;
 }
   
    public static void main(String[] args) {
        Scanner s=new Scanner(System.in);
        System.out.println("Enter the  start value");
        int start=s.nextInt();
        System.out.println("Enter the end value");
        int end=s.nextInt();
        int num=end;
        int last=-1;
        while(start<=num){
            if(isprime(num)){
              last=num;
              break;
            }
            num--;
        }
        System.out.println("Largest prime number "+last);
    }
}
        
OUTPUT:

Enter the  start value
2
Enter the end value
20
Largest prime number 19



````
## 98.Print all prime numbers up to n using a while loop. 

````java[]
import java.util.*;
public class Main {
         public static boolean isprime(int num){
             if(num<2){
                 return false;
             }
            int i=2;
        while(i<=num/2){
        if(num%i==0){
            return false;
        }
        i++;
   } 
        return true;
 }
   
    public static void main(String[] args) {
        Scanner s=new Scanner(System.in);
        System.out.println("Enter the value");
        int n=s.nextInt();
        int num=2;
        while(num<=n){
            if(isprime(num)){
                System.out.print(num+" ");
            }
            num++;
        }
    }
}
        
        
        

OUTPUT:

Enter the value
20
2 3 5 7 11 13 17 19 

````

## 99.Check if a number is prime using while loop. 

````java[]

import java.util.*;
public class Main {

   
    public static void main(String[] args) {
        Scanner s=new Scanner(System.in);
        System.out.println("Enter the value");
        int n=s.nextInt();
        int flag=0;
        int i=2;
        while(i<=n/2){
        if(n%i==0){
            flag=1;
            break;
        }
        i++;
        }
        
        if(flag==0){
            System.out.println(n +" is prime number");
        }
        else{
            System.out.println(n+" is not prime number");
        }
    }
    }

OUTPUT:

Enter the value
11
11 is prime number


````

## 100.Implement a simple ATM menu using a while loop. 

````java[]



````
