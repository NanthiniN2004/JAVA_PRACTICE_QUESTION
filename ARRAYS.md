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



