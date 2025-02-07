## 1.Check whether a number is positive or negative.

````java[]

import java.util.*;
public class Main {

   
    public static void main(String[] args) {
        Scanner s=new Scanner(System.in);
        System.out.println("Enter the value");
        int n=s.nextInt();
        if(n>0){
            System.out.println(n +" is positive");
        }
         else{
            System.out.println(n+" is negative");
        }
    }
    
}

OUTPUT:

Enter the value
-6
-6 is negative

````

##  2.Check whether a number is even or odd. 
````java[]

import java.util.*;
public class Main {

   
    public static void main(String[] args) {
        Scanner s=new Scanner(System.in);
        System.out.println("Enter the value");
        int n=s.nextInt();
        if(n%2==0){
            System.out.println(n +" is even");
        }
         else{
            System.out.println(n+" is odd");
        }
    }
    
}

output:

Enter the value
80
80 is even

````
## 3.Check whether a number is divisible by 3 and 5. 
````java[]

import java.util.*;
public class Main {

   
    public static void main(String[] args) {
        Scanner s=new Scanner(System.in);
        System.out.println("Enter the value");
        int n=s.nextInt();
        if(n%3==0 && n%5==0){
            System.out.println(n +" is Divisible by 3 and 5");
        }
         else{
            System.out.println(n+" is not Divisible by 3 and 5");
        }
    }
    
}

output:

Enter the value
15
15 is Divisible by 3 and 5


````
## 4.Find the largest of three numbers.

````java[]

import java.util.*;
public class Main {

   
    public static void main(String[] args) {
        Scanner s=new Scanner(System.in);
        System.out.println("Enter the value");
        int a=s.nextInt();
         int b=s.nextInt();
          int c=s.nextInt();
        if(a>b && a>c){
            System.out.println(a +" is largets Element");
        }
         else if(b>a && b>c){
            System.out.println(b+" is largets Element");
        }
        else{
            System.out.println(c+" is largets Element");
        }
    }
    
}

OUTPUT:

Enter the value
9
1
5
9 is largets Element

````

## 5.Check whether a number is a prime number (or)  11.Check if a number is prime or not using a simple loop. 

````java[]

import java.util.*;
public class Main {

   
    public static void main(String[] args) {
        Scanner s=new Scanner(System.in);
        System.out.println("Enter the value");
        int n=s.nextInt();
        int flag=0;
        for(int i=2;i<=n/2;i++){
        if(n%i==0){
            flag=1;
            break;
        }
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

##  6.Check whether a year is a leap year. 

````java[]
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	     int n=s.nextInt();
	     if(n%4 ==0 || (n%400==0 && (n%100 !=0))){
	         System.out.println( "ít is leap year" );
	     
	     }
	     else{
	         System.out.println("not leap year");
	     }
	    
		}
	}

output:

2020
ít is leap year

````

## 7.Find the greatest of four numbers. 

````java[]

import java.util.*;
public class Main {

   
    public static void main(String[] args) {
        Scanner s=new Scanner(System.in);
        System.out.println("Enter the value");
        int a=s.nextInt();
         int b=s.nextInt();
          int c=s.nextInt();
          int d=s.nextInt();
        if(a>b && a>c && a>d){
            System.out.println(a +" is largets Element");
        }
         else if(b>a && b>c && b>d){
            System.out.println(b+" is largets Element");
        }
        else if(c>a && c>b && c>d)
        {
            System.out.println(c+" is largets Element");
        }
        else{
            System.out.println(d+" is largets Element");
        }
    }
    
}

OUTPUT:

Enter the value
9
5
1
10
10 is largets Element

````

## 8.Check if a number is a palindrome. 

````java[]

import java.util.*;
public class Main {

   
    public static void main(String[] args) {
        Scanner s=new Scanner(System.in);
        System.out.println("Enter the value");
        int n=s.nextInt();
        int temp=n;
        int b=0;
        while(n!=0){
            int a=n%10;
            b=b*10+a;
            n/=10;
        }
        if(temp==b){
            System.out.println("number is palindrome");
        }
        else{
            System.out.println("number is not palindrome");
        }
    
    }
    
}


OUTPUT:

Enter the value
898
number is palindrome

````

##  9.Check whether a character is a vowel or consonant. 

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the character");
	     char ch=s.next().charAt(0);
	     if((ch>='a'&& ch<='z')||( ch>='A' && ch<='Z')){
	         if((ch=='a' ||ch=='e' || ch=='i' ||ch=='o'||ch=='u') || (ch=='A' ||ch=='E' || ch=='I' ||ch=='O'||ch=='U')){
	             System.out.println("vowels");
	         }
	     }
	     else{
	         if(ch>='0' && ch<='9'){
	             System.out.println("numbers");
	         }
	         else{
	             System.out.println("symbol");
	         }
	     }
		}
	}


OUTPUT:

Enter the character
o
vowels


````

##  10.Find the smallest of three numbers. 

````java[]

import java.util.*;
public class Main {

   
    public static void main(String[] args) {
        Scanner s=new Scanner(System.in);
        System.out.println("Enter the value");
        int a=s.nextInt();
         int b=s.nextInt();
          int c=s.nextInt();
        if(a<b && a<c){
            System.out.println(a +" is Smallest Element");
        }
         else if(b<a && b<c){
            System.out.println(b+" is Smallest Element");
        }
        else{
            System.out.println(c+" is Smallest Element");
        }
    }
    
}

OUTPUT:

Enter the value
50
44
20
20 is Smallest Element

````

## 12.Check if a number is perfect or not. 

````java[]


import java.util.*;
public class Main {

   
    public static void main(String[] args) {
        Scanner s=new Scanner(System.in);
        System.out.println("Enter the value");
        int n=s.nextInt();
        int temp=n;
        int sum=0;
        for(int i=1;i<n;i++){
            int rem=n%i;
          if(rem==0){
              sum+=i;
          }
    
        }
        if(temp==sum){
            System.out.println(n+ " is Perfect number");
        }
        else{
            System.out.println(n+" is not perfect number");
        }
    
    }
    
}

OUTPUT:

Enter the value
29
28 is Perfect number

````

## 13.Find whether a number is Armstrong or not. 

````java[]

import java.util.*;
import java.lang.*;
public class Main
{
	public static void main(String[] args) {
   Scanner s=new Scanner(System.in);
   int n=s.nextInt();
   int temp=n;
    int count=(int)Math.log10(n)+1;
	 int a;
	 double result=0;
	while(n!=0){
	     a=n%10;
         result+=Math.pow(a,count);
	     n/=10;
	}
	
	if(temp==result){
	    System.out.println("Amstrong ");
	    
	}
	else{
	     System.out.println("not Amstrong");
	}
}
}


output:

153
Amstrong 


````





