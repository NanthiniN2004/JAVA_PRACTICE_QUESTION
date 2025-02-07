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

## 5.Check whether a number is a prime number. 


