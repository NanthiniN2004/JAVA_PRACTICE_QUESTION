## 141.Print a Fibonacci sequence using a recursive function.

````java[]

import java.util.*;
public class Main
{  
    
    public static int fib(int n){
        if(n<=1){
            return n;
        }
        return fib(n-1)+fib(n-2);
    }
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
		System.out.println("Enter the number");
		int n=s.nextInt();
		System.out.println("Fibnacci of number");
		for(int i=0;i<n;i++){
		    System.out.print(fib(i)+" ");
		}
	}
}

OUTPUT:

Enter the number
10
Fibnacci of number
0 1 1 2 3 5 8 13 21 34 
````


## 142.Use a loop to generate prime numbers in a given range.

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

## 143.Implement linear search for a number in an array.

````JAVA[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
		Scanner s=new Scanner(System.in);
		System.out.println("Enter the size of the arra");
		int n=s.nextInt();
		int[] a=new int[n];
		System.out.println("Enter the element");
		for(int i=0;i<n;i++){
		    a[i]=s.nextInt();
		}
		System.out.println("Enter the target");
		int target=s.nextInt();
		int flag=0;
		for(int i=0;i<n;i++){
		    if(a[i]==target){
		       flag=1;
		    }
		    
		}	    
		    if(flag==1){
		         System.out.println("Element is found");
		    }
		    else{
		        System.out.println("Element is not found");
		    }
	
	}
}


output:

Enter the size of the arra
5
Enter the element
80
50
10
40
90
Enter the target
50
Element is found

````

## 144.Implement binary search in a sorted array

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
		Scanner s=new Scanner(System.in);
		System.out.println("Enter the size of the array");
		int n=s.nextInt();
		int[] a=new int[n];
		System.out.println("Enter the element");
		for(int i=0;i<n;i++){
		    a[i]=s.nextInt();
		}
		System.out.println("Enter the target");
		int target=s.nextInt();
		int start=0;
		int end=a.length-1;
		int flag=0;
		while(start<=end){
		    int mid=(start+end)/2;
		    if(a[mid]==target){
		        flag=1;
		        System.out.println("Element Found: "+mid);
		        break;
		    }
		    else if(a[mid]<target){
		        start=mid+1;
		    }
		    else{
		        end=mid-1;
		    }
		}
		if(flag==0){
		    System.out.println("Element Not found");
		}
	}
}


OUTPUT:

Enter the size of the arra
5
Enter the element
20
30
40
50
60
Enter the target
50
Element Found: 3


````

