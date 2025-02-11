## 141.Print a Fibonacci sequence using a recursive function (or)  146.Implement recursive Fibonacci sequence. 

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

##  145.Perform matrix multiplication using nested loops.

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
		Scanner s=new Scanner(System.in);
	    System.out.println("Enter the number of rows");
	    int row=s.nextInt();
	    System.out.println("Enter the number of column");
	    int col=s.nextInt();
	    int[][] a=new int[row][col];
	    int[][] b=new int[row][col];
	    int[][] mul=new int[row][col];
	    System.out.println("Enter the first matrix element");
	    for(int i=0;i<row;i++){
	        for(int j=0;j<col;j++){
	            a[i][j]=s.nextInt();
	        }
	    }
	     System.out.println("Enter the  second matrix element");
	    for(int i=0;i<row;i++){
	        for(int j=0;j<col;j++){
	            b[i][j]=s.nextInt();
	        }
	    }
	    
	     for(int i=0;i<row;i++){
	        for(int j=0;j<col;j++){
	            for(int k=0;k<col;k++)
	            mul[i][j] +=a[i][k]*b[k][j];
	        }
	    }
	    
	    
	    System.out.println("Multipliction of the matrix");
	     for(int i=0;i<row;i++){
	        for(int j=0;j<col;j++){
	          System.out.print(mul[i][j]+" ");
	        }
	        System.out.println();
	    }
	}
}

OUTPUT:

Enter the number of rows
2
Enter the number of column
2
Enter the first matrix element
1
2
3
4
Enter the  second matrix element
5
6
7
8
Multipliction of the matrix
19 22 
43 50 

````

## 147.Implement recursive factorial calculation. 

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

## 148.Find the largest number using a method and return the result. 

````java[]

import java.util.*;
public class Main
{
    
    public static int largets(int a,int b,int c){
        if(a>b && a>c){
            return a;
        }
        else if(b>a && b>c){
            return b;
        }
        else{
            return c;
        }
    }
	public static void main(String[] args) {
		System.out.println("Enter the value of a and b and c");
		Scanner s=new Scanner(System.in);
		int a=s.nextInt();
		int b=s.nextInt();
		int c=s.nextInt();
		int result=	largets(a,b,c);
		System.out.println("largets element "+result);
	
	}
}


OUTPUT:

Enter the value of a and b and c
77
71
55
largets element 77

````

## 149.Count the occurrence of each character in a string. 

````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
		System.out.println("Enter the String");
		Scanner s=new Scanner(System.in);
		String str=s.nextLine();
		int[] count=new int[256];
	  for(char ch:str.toCharArray()){
	      count[ch]++;
	  }
	  for(int i=0;i<256;i++){
	      if(count[i]>0){
	          System.out.println((char)i +": "+count[i]);
	      }
	  }
		
	}
}

OUTPUT:

Enter the String
Nanthii ni
N: 1
a: 1
h: 1
i: 2
n: 2
t: 1

````

## 150.Implement an input validation program with a loop. 
````java[]

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	
		Scanner s=new Scanner(System.in);
	   int number;
	   while(true){
	       	System.out.println("Enter the positive number");
	       if(s.hasNextInt()){
	           number=s.nextInt();
	           if(number>0){
	               break;
	           }
	           else{
	               System.out.println("Error: Please enter positive number");
	           }
	       }
	       else{
	           System.out.println("invalid input: please enter integer");
	           s.next();
	       }
	   }
	   System.out.println("valid input received "+ number);
		
	}
}

OUTPUT:

Enter the positive number
abc
invalid input: please enter integer
Enter the positive number
-6
Error: Please enter positive number
Enter the positive number
51
valid input received51


````
## 151.Check if a number is an Armstrong number recursively. 

````java[]



````
## 152.Implement a switch case that calculates tax based on income. 
````java[]

````
## 153.Implement a stack data structure using control flow statements.

````java[]

import java.util.Scanner;

class Stack {
    private int top;
    private int size;
    private int[] a;

   
    public Stack(int size) {
        this.size = size;
        this.a = new int[size]; 
        this.top = -1; 
    }

    public void push(int data) {
        if (top == size - 1) {
            System.out.println("Stack is full! Cannot push " + data);
        } else {
            a[++top] = data;
            System.out.println("Pushed: " + data);
        }
    }

   
    public void pop() {
        if (top == -1) {
            System.out.println("Stack is empty! Nothing to pop.");
        } else {
            System.out.println("Popped: " + a[top--]);
        }
    }

 
    public void peek() {
        if (top == -1) {
            System.out.println("Stack is empty! No top element.");
        } else {
            System.out.println("Top element: " + a[top]);
        }
    }

    public void display() {
        if (top == -1) {
            System.out.println("Stack is empty.");
        } else {
            System.out.print("Stack elements: ");
            for (int i = top; i >= 0; i--) {
                System.out.print(a[i] + " ");
            }
            System.out.println();
        }
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);

        System.out.print("Enter the size of the stack: ");
        int size = s.nextInt();

        Stack stack = new Stack(size);

        while (true) {
            System.out.println("\n1. Push  2. Pop  3. Peek  4. Display  5. Exit");
            System.out.print("Choose an option: ");
            int choice = s.nextInt();

            if (choice == 1) {
                System.out.print("Enter value to push: ");
                int value = s.nextInt();
                stack.push(value);
            } else if (choice == 2) {
                stack.pop();
            } else if (choice == 3) {
                stack.peek();
            } else if (choice == 4) {
                stack.display();
            } else if (choice == 5) {
                System.out.println("Exiting...");
                break;
            } else {
                System.out.println("Invalid choice! Try again.");
            }
        }
    }
}

OUTPUT:

Enter the size of the stack: 5

1. Push  2. Pop  3. Peek  4. Display  5. Exit
Choose an option: 1
Enter value to push: 20
Pushed: 20

1. Push  2. Pop  3. Peek  4. Display  5. Exit
Choose an option: 1
Enter value to push: 30
Pushed: 30

1. Push  2. Pop  3. Peek  4. Display  5. Exit
Choose an option: 1
Enter value to push: 40
Pushed: 40

1. Push  2. Pop  3. Peek  4. Display  5. Exit
Choose an option: 1
Enter value to push: 50
Pushed: 50

1. Push  2. Pop  3. Peek  4. Display  5. Exit
Choose an option: 2
Popped: 50

1. Push  2. Pop  3. Peek  4. Display  5. Exit
Choose an option: 4
Stack elements: 40 30 20 

1. Push  2. Pop  3. Peek  4. Display  5. Exit
Choose an option: 5
Exiting...



````
## 154.Implement a queue using loops and conditional statements. 

````java[]

import java.util.*;
class Queue{
    int size,front,rear;
    int a[];
    public Queue(int size){
        this.size=size;
        this.a=new int[size];
        this.front=-1;
        this.rear=-1;
    }
    
    public void enqueue(int data){
        if(rear==size-1){
            System.out.println("Queue full");
        }
        else{
            if(front==-1){
                front=0;
            }
            a[++rear]=data;
            System.out.println("Enqueue " + data);
        }
    }
    public void dequeue(){
        if(front==-1 || front>rear){
            System.out.println("Queue empty");
            
        }
        else{
            System.out.println("Dequeue " +a[front++]);
        }
    }
    public void display(){
           for(int i=front;i<=rear;i++) {
          System.out.println(" Display the elements "+a[i]);
        
    }
    }
}

public class Main{
    public static void main(String args[]){
        Scanner s=new Scanner(System.in);
         System.out.print("Enter the size of the queue: ");
        int size = s.nextInt();

        Queue q = new Queue(size);

        while (true) {
            System.out.println("\n1. Enqueue  2. Dequeue   3. Display  4. Exit");
            System.out.print("Choose an option: ");
            int choice = s.nextInt();

            if (choice == 1) {
                System.out.print("Enter value to enqueue: ");
                int value = s.nextInt();
                q.enqueue(value);
            } else if (choice == 2) {
                q.dequeue();
          
            } else if (choice == 3) {
                q.display();
            } else if (choice == 4) {
                 System.out.println("Exiting...");
                break;
            } else {
                System.out.println("Invalid choice! Try again.");
            }
        }
    }
}


OUTPUT:

Enter the size of the queue: 3

1. Enqueue  2. Dequeue   3. Display  4. Exit
Choose an option: 1
Enter value to enqueue: 10
Enqueue 10

1. Enqueue  2. Dequeue   3. Display  4. Exit
Choose an option: 1
Enter value to enqueue: 20
Enqueue 20

1. Enqueue  2. Dequeue   3. Display  4. Exit
Choose an option: 3
 Display the elements 10
 Display the elements 20

1. Enqueue  2. Dequeue   3. Display  4. Exit
Choose an option: 2
Dequeue 10

1. Enqueue  2. Dequeue   3. Display  4. Exit
Choose an option: 3
 Display the elements 20

1. Enqueue  2. Dequeue   3. Display  4. Exit
Choose an option: 4
Exiting...


````
## 155.Create a simple bank account with multiple operations. 

````java[]

package Nanthu;
import java.util.*;
 class BankAccount{
	  String AccountHolderName;
	  String AccountNumber;
	  double balance;
	  
	  BankAccount(String AccountHolderName,String AccountNumber,double balance){
		  this.AccountHolderName=AccountHolderName;
		  this.AccountNumber=AccountNumber;
		  this.balance=balance;
	  }
	  
	  public void deposit(double amount) {
		  if(amount>0) {
			  balance+=amount;
			  System.out.println("Deposit $ "+amount);
		  }
		  else {
			  System.out.println("invalid amount");
		  }
	  }
	  
	  public void withdraw(double amount) {
		  if(amount>0 && amount<=balance) {
			  balance-=amount;
			  System.out.println("Withdraw $ "+ balance);
		  }
		  else {
			  System.out.println("Invalid amount or insufficient balance");
		  }
	  }
	  
	  public void checkbalance() {
		  System.out.println("Balance Amount $ : " + balance);
	  }
	  public void detail() {
		  System.out.println("Account Holder Name: " + AccountHolderName);
		  System.out.println("Account Number: " + AccountNumber);
		  System.out.println("Balance Amount $ : " + balance);
	  }
 }
public class Main {

	public static void main(String[] args) {
	 Scanner s=new Scanner(System.in);
	 System.out.println("Enter the Account Holder Name");
	 String AccountHolderName=s.nextLine();
	 System.out.println("Enter the Account Number");
	 String AccountNumber=s.nextLine();
	 System.out.println("Enter the Initial Balance");
	 double  balance=s.nextDouble();
	 BankAccount b=new BankAccount(AccountHolderName,AccountNumber,balance);
     while(true) {
    	 System.out.println("\nChoose an operation:");
         System.out.println("1. Deposit");
         System.out.println("2. Withdraw");
         System.out.println("3. Check Balance");
         System.out.println("4. Account Details");
         System.out.println("5. Exit");
         System.out.print("Enter choice: ");
         int choice = s.nextInt();
         
         switch(choice) {
         case 1:
        	 System.out.println("Enter the deposit amount");
        	 double amount=s.nextDouble();
        	 b.deposit(amount);
        	 break;
         
         case 2:
        	 System.out.println("Enter the withdraw amount");
        	 double withdrawamount=s.nextDouble();
        	 b.deposit(withdrawamount);
        	 break;
         
         case 3:
        	 b.checkbalance();
        	 break;
        
         case 4:
        	 b.detail();
        	 break;
        	 
         case 5:
        	 System.out.println("Thank you");
        	 return;
        default:
        	System.out.println("invalid choice, please Enter valid choice");
        
     }
	}
	}

}


OUTPUT:

Enter the Account Holder Name
Nanthini
Enter the Account Number
957623
Enter the Initial Balance
2000

Choose an operation:
1. Deposit
2. Withdraw
3. Check Balance
4. Account Details
5. Exit
Enter choice: 1
Enter the deposit amount
1000
Deposit $ 1000.0

Choose an operation:
1. Deposit
2. Withdraw
3. Check Balance
4. Account Details
5. Exit
Enter choice: 3
Balance Amount $ : 3000.0

Choose an operation:
1. Deposit
2. Withdraw
3. Check Balance
4. Account Details
5. Exit
Enter choice: 5
Thank you


````
## 156.Implement a simple ticket reservation system. 

````java[]


package Nanthu;
import java.util.*;
 class Ticket{
	  String passengername;
	  String Trainnumber;
	  int seatnumber;
	  boolean isReserved;
	  
	  Ticket(String passengername,String Trainnumber,int seatnumber){
		  this.passengername=passengername;
		  this.Trainnumber=Trainnumber;
		  this.seatnumber=seatnumber;
		  this.isReserved=true;
	  }
	  
	  public void cancelTicket() {
		  if(isReserved) {
			  isReserved=false;
			  System.out.println("Reservation cancel for this seat "+seatnumber);
		  }
		  else {
			  System.out.println("No Reservation found");
		  }
	  }
	  
	  public void detail() {
		  if(isReserved) {
		  System.out.println("Passenger Name: " + passengername);
		  System.out.println("Train Number: " + Trainnumber);
		  System.out.println("Seat number: " + seatnumber);
		  }
		  else{
			  System.out.println("No Reservation found");
		  }
	  }
 }
public class Main1 {

	public static void main(String[] args) {
		ArrayList<Ticket> booking=new ArrayList<>();
	 Scanner s=new Scanner(System.in);
	 System.out.println("Enter the Passenger Name");
	 String passengername=s.nextLine();
	 System.out.println("Enter the Train Number");
	 String Trainnumber=s.nextLine();
	 System.out.println("Enter the Seat Number");
	 int  seatnumber=s.nextInt();
       Ticket b=new Ticket(passengername,Trainnumber,seatnumber);
     while(true) {
    	 System.out.println("\nChoose an operation:");
         System.out.println("1. Booking Ticket");
         System.out.println("2. Cancel Ticket");
         System.out.println("3. View Reservation");
         System.out.println("4. Exit");
         System.out.print("Enter choice: ");
         int choice = s.nextInt();
         
         switch(choice) {
         case 1:
             booking.add(new Ticket(passengername, Trainnumber,seatnumber));
             System.out.println("Ticket booked!");
             break;
         
         case 2:
        	b.cancelTicket();
        	 break;
         
         case 3:
        	 b.detail();
        	 break;
        	 
         case 4:
        	 System.out.println("Thank you");
        	 return;
        default:
        	System.out.println("invalid choice, please Enter valid choice");
        
     }
	}
	}

}

OUTPUT:

Enter the Passenger Name
Nanthini
Enter the Train Number
51
Enter the Seat Number
70

Choose an operation:
1. Booking Ticker
2. Cancel Ticket
3. View Reservation
4. Exit
Enter choice: 1
Ticket booked!

Choose an operation:
1. Booking Ticker
2. Cancel Ticket
3. View Reservation
4. Exit
Enter choice: 3
Passenger Name: Nanthini
Train Number: 51
Seat number: 70

Choose an operation:
1. Booking Ticker
2. Cancel Ticket
3. View Reservation
4. Exit
Enter choice: 4
Thank you



````
# 157.Write a program to calculate power using recursion. 

````java[]


````
## 158.Create a number guessing game with loops and conditions. 
````java[]



````
## 159.Print a checkerboard pattern using nested loops. 

````java[]


````
## 160.Implement a vending machine system using switch statements.

````java[]



````
