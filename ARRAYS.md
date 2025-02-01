## 1)SUM OF ELEMENTS
```java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
		System.out.println("Enter the size of the array");
		int n=s.nextInt();
		int a[]=new int[n];
		System.out.println("Enter the Elements");
		for(int i=0;i<n;i++){
		    a[i]=s.nextInt();
		}
		
		int sum=0;
		for(int i=0;i<n;i++){
		    sum+=a[i];
		}
		System.out.println("Sum of the element "+sum);
	}
}


output

Enter the size\ of the array
5
Enter the Elements
8
2
5
1
9
Sum of the element 25

````

##  2)FIND MINIMUM AND MAXIMUM ELEMENT IN ARRAY

````java[]
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
		System.out.println("Enter the sizee of the array");
		int n=s.nextInt();
		int a[]=new int[n];
		System.out.println("Enter the Elements");
		for(int i=0;i<n;i++){
		    a[i]=s.nextInt();
		}
		
		int min=a[0];
		int max=a[0];
		for(int i=0;i<n;i++){
		   if(min>a[i]){
		       min=a[i];
		   }
		   if(max<a[i]){
		       max=a[i];
		   }
		}
		System.out.println("Maximum of the element "+max);
		
		System.out.println("Minimum of the element "+min);
	}
}


output

Enter the sizee of the array
5
Enter the Elements
77
71
51
55
63
Maximum of the element 77
Minimum of the element 51


````

##  3) REVERSE AN ARRAY

````java[]
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
		System.out.println("Enter the size of the array");
		int n=s.nextInt();
		int a[]=new int[n];
		System.out.println("Enter the Elements");
		for(int i=0;i<n;i++){
		    a[i]=s.nextInt();
		}
		
		System.out.println("After Reverse Element");
	   for(int i=n-1;i>=0;i--){
	       System.out.print(a[i]+" ");
	   }
	}
}

output:

Enter the size of the array
5
Enter the Elements
8
2
5
1
6
After Reverse Element
6 1 5 2 8

````

##  4) FIND THE DUPLICATE ELEMENT IN AN ARRAY

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
		System.out.println("Enter the size of the array");
		int n=s.nextInt();
		int a[]=new int[n];
		System.out.println("Enter the Elements");
		for(int i=0;i<n;i++){
		    a[i]=s.nextInt();
		}
		
		System.out.println("Duplicate value");
	 for(int i=0;i<n;i++){
	     for(int j=i+1;j<n;j++){
	     if(a[i]==a[j]){
	         System.out.println(a[j]);
	}
}
}
	     }
	 }

output:

Enter the size of the array
9
Enter the Elements
1
2
3
4
2
7
8
8
1
Duplicate value
1
2
8

````

## 5) FIND THE KTH LARGEST ELEMENT

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
		System.out.println("Enter the size of the array");
		int n=s.nextInt();
		int a[]=new int[n];
		System.out.println("Enter the Elements");
		for(int i=0;i<n;i++){
		    a[i]=s.nextInt();
		}
        int k=s.nextInt();
        for(int i=0;i<n;i++){
            for(int j=i+1;j<n;j++){
                if(a[i]<a[j]){
                int temp=a[i];
                a[i]=a[j];
                a[j]=temp;
            }
            }
        }
        System.out.println("After Swapping");
        for(int i=0;i<n;i++){
            System.out.print(a[i]+" ");
        }
        System.out.println(k+"th Largest Element"+a[k-1]);
	     }
	 }


OUTPUT:

Enter the size of the array
8
Enter the Elements
51
55
71
77

115
35
37
99
3
After Swapping
115 99 77 71 55 51 37 35
3th Largest Element77

````

## 6) CHECK IF A GIVEN NUMBER IS PRESENT IN ARRAY
````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
		System.out.println("Enter the size of the array");
		int n=s.nextInt();
		int a[]=new int[n];
		System.out.println("Enter the Elements");
		for(int i=0;i<n;i++){
		    a[i]=s.nextInt();
		}
        System.out.println("Enter the number you want to check");
        int k=s.nextInt();
        boolean found=false;
        for(int i=0;i<n;i++){
            if(a[i]==k){
                found=true;
            }
        }
        if(found==true){
            System.out.println("Element is found");
        }
        else{
            System.out.println("Element is not found");
        }
	     }
	 }

OUTPUT:

Enter the size of the array
4
Enter the Elements
7
1
4
9
Enter the number you want to check
2
Element is not found


````


## FIND THE UNIQUE VALUE

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
		System.out.println("Enter the size of the array");
		int n=s.nextInt();
		int a[]=new int[n];
		System.out.println("Enter the Elements");
		for(int i=0;i<n;i++){
		    a[i]=s.nextInt();
		}
		
		System.out.println("unique value");
	 for(int i=0;i<n;i++){
	     int count=0;
	     for(int j=0;j<n;j++){
	     if(a[i]==a[j]){
	        count++;
	}
}
if(count==1){
    System.out.println(a[i]);
}
}
	     }
	 }

OUTPUT:
Enter the size of the array
6
Enter the Elements
5
2
5
4
1
4
unique value
2
1

````

