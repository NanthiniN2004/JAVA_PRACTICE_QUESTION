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
## 14.Calculate the factorial of a number using recursion.

````java[]

import java.util.*;
public class Main
{
    public static int factorial(int n){
		    	if(n==0 || n==1){
		    	    return 1;
		    	}
		    	return n*factorial(n-1);
		
		}
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
		System.out.println("Enter the value");
		int n=s.nextInt();
		int result=factorial(n);
		System.out.println(n+ " factorial is "+result);
	
	}
}


output:

Enter the value
7
7 factorial is 5040


````

## 15.Check whether a number is an automorphic number.

````java[]


import java.util.*;

public class Main
{
	public static void main(String[] args) {
     Scanner s=new Scanner(System.in);
     int n=s.nextInt();
     int sqr=n*n;
     while(n>0){
         if(n%10!=sqr%10){
             System.out.println("Not Automorphic number");
             break;
         }
         n/=10;
         sqr/=10;
     }
     if(n==0){
         System.out.println(" Automorphic number");
     }
	}
}

OUTPUT:

25
 Automorphic number


````

## 16.Find if a number is a Fibonacci number.

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
      Scanner s=new Scanner(System.in);
      System.out.println("Ënter the value of n");
     int n=s.nextInt();
         int a=0;
         int b=1;
         System.out.println(a);
         System.out.println(b);
		for(int i=0;i<=n;i++){
		   	
		   	int c=a+b;
		   	a=b;
            b=c;
            
		 System.out.print(c+" ");
		}

	}
}


OUTPUT:

Ënter the value of n
7
0
1
1 2 3 5 8 13 21 34

````

## 17.Count the number of digits in a number.

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
      Scanner s=new Scanner(System.in);
      System.out.println("Ënter the value of n");
     int n=s.nextInt();
        int count=0;
        while(n!=0){
            int a=n%10;
            count++;
            n/=10;
        }
        System.out.println(" count of the digit "+count);

	}
}


OUTPUT:


Ënter the value of n
69524
 count of the digit 5


````

## 18.Check whether a string is a palindrome.  (or)  31.Check whether a string is a valid palindrome.

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
      Scanner s=new Scanner(System.in);
      System.out.println("Ënter the String");
      String str=s.next();
      String rev="";
      for(int i=str.length()-1;i>=0;i--){
          rev+=str.charAt(i);
      }
      
      if(rev.equals(str)){
      System.out.println("Palindrome");
      }
      else{
          System.out.println("Not Palindrome");
      }
	}
}


OUTPUT:

Ënter the String
amma
Palindrome

````

## 19.Check if a string is an anagram of another string

````JAVA[]


import java.util.*;
public class Main
{
	public static void main(String[] args) {
      Scanner s=new Scanner(System.in);
      System.out.println("Ënter the String");
      String str1=s.next();
      System.out.println("Ënter the string ");
      String str2=s.next();
      str1=str1.toLowerCase();
      str2=str2.toLowerCase();
      if(str1.length()!=str2.length())
      {
          System.out.println("both String not anagram");
          
      }
      else{
          char[] String1=str1.toCharArray();
          char[] String2=str2.toCharArray();
          
          Arrays.sort(String1);
          Arrays.sort(String2);
          if(Arrays.equals(String1, String2)==true){
              System.out.println("both String is Anagram");
          }
          else{
              System.out.println("both String not anagram");
          }
      }
	}
}



OUTPUT:

Ënter the String
brag    Grab
Ënter the string 
Brag

both String is Anagram

````

##  20.Determine if a number is a perfect square.

````JAVA[]

import java.util.*;
import java.lang.*;
public class Main{
    public static void main(String args[]){
        Scanner s=new Scanner(System.in);
        System.out.println("Ënter the value");
        int n=s.nextInt();
        int a=(int)Math.sqrt(n);
        if((a*a)==n){
            System.out.println("Perfect Square");
        }
        else{
             System.out.println(" Not Perfect Square");
        }
    }
}

OUTPUT:

Ënter the value
64
Perfect Square


````

## 21.Check whether a number is a prime number within a range  (OR)  23.Print all prime numbers in a range using nested loops. (or) 35.Print prime numbers within a range using nested conditions.

````JAVA[]

import java.util.*;
import java.lang.*;
public class Main{
    public static boolean isPrime(int n){
            if(n==1){
                return false;
            }
            for(int i=2;i<=n/2;i++){
            if(n%i==0){
                return false;
            }
            }
            return true;
        }
        public static void range(int start,int end){
            System.out.println(" Prime number between"+ start +"to"+end);
            for(int i=start;i<end;i++){
                if(isPrime(i)){
                    System.out.print(i+" ");
                }
            }
             System.out.println();

            }
    public static void main(String args[]){
        Scanner s=new Scanner(System.in);
        System.out.println("Ënter the Range");
        int start=s.nextInt();
        int end=s.nextInt();
        range(start,end);
        
        
    }
}

OUTPUT:

Ënter the Range
10
50
 Prime number between 10to50
11 13 17 19 23 29 31 37 41 43 47 

````

##  22.Find the largest number among n numbers using a nested if-else.

````java[]

import java.util.*;

public class Main
{
	public static void main(String[] args) {
		Scanner s=new Scanner(System.in);
		System.out.println("Enter the value of n");
		int n=s.nextInt();
		System.out.println("Enter the element");
		int max=s.nextInt();
		for(int i=1;i<n;i++){
		    int ele=s.nextInt();
		    if(max<ele){
		        max=ele;
		    }
		}
		System.out.println(" Largest Element "+max);
	}
}


OUTPUT:

Enter the value of n
7
Enter the element
51
55
71
77
63
115
101
 Largest Element 115

````

## 24.Find all the divisors of a number.

````JAVA[]

import java.util.*;

public class Main
{
	public static void main(String[] args) {
		Scanner s=new Scanner(System.in);
		System.out.println("Enter the value of n");
		int n=s.nextInt();
		System.out.println("Divisor of a number");
	   for(int i=1;i<=n;i++){
	       if(n%i==0){
	           System.out.print(i+" ");
	       }
	   }
	}
}


OUTPUT:

Enter the value of n
28
Divisor of a number
1 2 4 7 14 28

````

## 25.Check if a number is a perfect number within a range.

````JAVA[]

import java.util.*;
import java.lang.*;
public class Main{
    public static boolean isPerfect(int n){
        int a=(int)Math.sqrt(n);
        if((a*a)==n){
            return true;
        }
        else{
             return false;
        }
        }
        public static void range(int start,int end){
            System.out.println(" Perfect number between "+ start +" to " +end);
            for(int i=start;i<end;i++){
                if(isPerfect(i)){
                    System.out.print(i+" ");
                }
            }
             System.out.println();

            }
    public static void main(String args[]){
        Scanner s=new Scanner(System.in);
        System.out.println("Ënter the Range");
        int start=s.nextInt();
        int end=s.nextInt();
        range(start,end);
        
        
    }
}


OUTPUT:

Ënter the Range
10
50
 Perfect number between10to50
16 25 36 49 


````
## 26.Check whether an integer is positive, negative, or zero.

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
        else if(n==0)
        {
                System.out.println(n+" is zero");
        }
         else{
            System.out.println(n+" is negative");
        }
    }
    
}

OUTPUT:

Enter the value
54
54 is positive


````

## 27.Find whether a number is a Fibonacci number within a range.

````JAVA[]

import java.util.*;
import java.lang.*;
public class Main{
    public static boolean fibnassi(int n){
       if(n==0 || n==1){
           return true;
       }
      int a=0,b=1,c=0;
		while(c<n){
		   	
		    c=a+b;
		   	a=b;
            b=c;

        }
        return c==n;
    }
        public static void range(int start,int end){
            System.out.println("Fibnassi number between "+ start +" to " +end);
            for(int i=start;i<end;i++){
                if(fibnassi(i)){
                    System.out.print(i+" ");
                }
            }
             System.out.println();

            }
    public static void main(String args[]){
        Scanner s=new Scanner(System.in);
        System.out.println("Ënter the Range");
        int start=s.nextInt();
        int end=s.nextInt();
        range(start,end);
        
        
    }
}

OUTPUT:

Ënter the Range
10
50
Fibnassi number between 10 to 50
13 21 34 

````

##  28.Print all leap years within a given range.

````JAVA[]

import java.util.*;
import java.lang.*;
public class Main{
    public static boolean leap(int n){
        if(n%4 ==0 || (n%400==0 && (n%100 !=0))){
	          return true;
	     }
	     else{
	         return false;
	     }
    }
        public static void range(int start,int end){
            System.out.println("Leap Year  between "+ start +" to " +end);
            for(int i=start;i<end;i++){
                if(leap(i)){
                    System.out.print(i+" ");
                }
            }
             System.out.println();

            }
    public static void main(String args[]){
        Scanner s=new Scanner(System.in);
        System.out.println("Ënter the Range");
        int start=s.nextInt();
        int end=s.nextInt();
        range(start,end);
        
        
    }
}

OUTPUT:

Ënter the Range
2000
2050
Leap Year  between 2000 to 2050
2000 2004 2008 2012 2016 2020 2024 2028 2032 2036 2040 2044 2048 


````

## 29.Find the GCD and LCM of two numbers.

````JAVA[]

import java.util.*;
public class Main
{
    public static int gcd(int n1,int n2)
    {
        while(n1!=n2){
            if(n1>n2){
                n1-=n2;
            }
            else{
                n2-=n1;
            }
        }
        return n1;
    }
    public static int lcm(int n1,int n2,int gcdvalue){
        return Math.abs(n1*n2)/gcdvalue;
    }
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
		System.out.println("Enter the number");
		int n1=s.nextInt();
		int n2=s.nextInt();
		System.out.println("gcd of " +n1+" and "+n2);
		 int gcdvalue=gcd(n1,n2);
		 System.out.println(gcdvalue);
		System.out.println("lcm of " +n1+" and "+n2);
		int lcmvalue=lcm(n1,n2,gcdvalue);
	   System.out.println(lcmvalue);
		
	}
}

OUTPUT:

Enter the number
20
30
gcd of 20 and 30
10
lcm of 20 and 30
60


````

## 30. Determine the type of a triangle based on its angles.

````JAVA[]

import java.util.*;
public class Main {

   
    public static void main(String[] args) {
        Scanner s=new Scanner(System.in);
        System.out.println("Enter the First Angle");
        int n1=s.nextInt();
        System.out.println("Enter the Second Angle");
         int n2=s.nextInt();
         System.out.println("Enter the Third Angle");
          int n3=s.nextInt();
          int sum=n1+n2+n3;
         if(sum==180){
        if(n1<90 && n2<90 && n3<90){
            System.out.println(" Acute Triangle ");
        }
         else if (n1==90 || n2==90 || n3==90){
            System.out.println(" Right Triangle ");
        }
        else{
            System.out.println(" Obtuse Triangle ");
        }
         }
         else{
             System.out.println(" Invalid");
         }
    }
    
}

OUTPUT:

Enter the First Angle
1000 
Enter the Second Angle
40
Enter the Third Angle
40
 Obtuse Triangle 


````

## 32.Check if a number is divisible by 7 or 11.

````jAVA[]

import java.util.*;
public class Main {

   
    public static void main(String[] args) {
        Scanner s=new Scanner(System.in);
        System.out.println("Enter the value");
        int n=s.nextInt();
        if(n%7==0 && n%11==0){
            System.out.println(n +" is Divisible by 7 and 11");
        }
         else{
            System.out.println(n+" is not Divisible by 7 and 11");
        }
    }
    
}

output:

Enter the value
77
77 is Divisible by 7 and 11

````

##  33.Print multiplication tables for a given number using nested loops.

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	Scanner s=new Scanner(System.in);
	int n=s.nextInt();

		for(int i=1;i<=10;i++){
		   		System.out.println(i+"*"+n+"="+(i*n));
		
		}

	
}
}

OUTPUT:

8
1*8=8
2*8=16
3*8=24
4*8=32
5*8=40
6*8=48
7*8=56
8*8=64
9*8=72
10*8=80


````

## 34.Identify if an alphabet character is uppercase, lowercase, or non-alphabet.

````JAVA[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	Scanner s=new Scanner(System.in);
	char ch=s.next().charAt(0);

	if(ch>='A' && ch<='Z'){
	    System.out.println("Given character is lower case");
	}
	else if(ch>='a' && ch<='z'){
	    System.out.println("Given character is upper case");
	}
	else{
	    System.out.println("Non alphabet");
	}

	
}
}

OUTPUT:

a
Given character is upper case


````

## 36.Determine if a given number is a valid credit card number.

````JAVA[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the card number");
	    long num=s.nextLong();
	   long sum=0;
	    boolean seconddigit=false;
	    while(num>0){
	        long digit=num%10;
	        num/=10;
	        if(seconddigit){
	            digit=digit*2;
	            if(digit>=10){
	                digit-=9;
	            }
	            sum+=digit;
	            seconddigit=!seconddigit;
	        }
	    }
	    if(sum%10==0){
	        System.out.println("valid card number");
	    }
	    else{
	        System.out.println("not valid number");
	    }
	}
}


OUTPUT:

Enter the card number
4532015112830366
valid card number

````

##  37.Check if a given day is a weekend or weekday.

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
		System.out.println("Enter the day");
		String day=s.next().toLowerCase();
		if(day.equals("sunday") || day.equals("saturday")){
		    System.out.println("Weekend");
		}
		else{
		    System.out.println("Weekday");
		}
		
	
	}
}


OUTPUT:

Enter the day
wednesday
Weekday

````
##  38.Check if a given date is valid or invalid.
````java[]

import java.util.*;
import java.time.LocalDate;
public class Main
{
    
    public static boolean valid(int date,int month,int year){
        try{
        LocalDate.of(year,month,date);
        return true;
        }
        catch(Exception e){
            return false;
        }
    }
	public static void main(String[] args) {
	 Scanner s=new Scanner(System.in);
	 System.out.println("Enter the year");
	 int year=s.nextInt();
	  System.out.println("Enter the month");
	 int month=s.nextInt();
	  System.out.println("Enter the date");
	 int date=s.nextInt();
	 
	 if(valid(date,month,year)){
	     System.out.println("valid date");
	 }
	 else{
	     System.out.println(" Not valid date");
	 }
	 
	}	
}

OUTPUT:

Enter the year
2025
Enter the month
2
Enter the date
9 29
 Not valid date

````

## 39.Find the day of the week for a given date. 
````java[]

import java.util.*;
import java.time.LocalDate;
import java.time.DayOfWeek;
public class Main
{
    

	public static void main(String[] args) {
	 Scanner s=new Scanner(System.in);
	 System.out.println("Enter the year");
	 int year=s.nextInt();
	  System.out.println("Enter the month");
	 int month=s.nextInt();
	  System.out.println("Enter the date");
	 int day=s.nextInt();
	 
	 try{
	 LocalDate date=LocalDate.of(year,month,day);
	 DayOfWeek week=date.getDayOfWeek();
	 System.out.println(" day of the week "+week);
	 }
	 catch(Exception e){
	     System.out.println("Invalid date");
	 }
	}	
}


OUTPUT:
Enter the year
2004
Enter the month
11
Enter the date
13
 day of the week SATURDAY

````

## 40.Check for a specific pattern in a string using if-else. 

````java[]


import java.util.*;
public class Main{
    public static void main(String args[]){
        Scanner s=new Scanner(System.in);
        System.out.println("Enter the string");
        String str=s.nextLine();
        System.out.println("Enter the pattern");
        String pat=s.nextLine();
        if(str.contains(pat)){
            System.out.println("pattern found");
        }
        else{
            System.out.println("pattern Not found");
        }
    }
}

OUTPUT:

Enter the string
xyzabcdef
Enter the pattern
abc
pattern found

````




