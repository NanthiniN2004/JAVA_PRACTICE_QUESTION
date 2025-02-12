## 181.Create a calculator that supports multiple operations (addition, subtraction, etc.).
````java[]

package sample;

import java.util.*;
public class Main9
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the two value");
	    int a=s.nextInt();
	    int b=s.nextInt();
		System.out.println("Enter the symbol");
		char c=s.next().charAt(0);
		switch(c){
		    case '+':
		        System.out.println("Addition: "+ (a+b));
		        break;
		     case '-':
		         System.out.println("Subtraction:"+ (a-b)); 
		        break;
		        
		    case '*':
		         System.out.println("Multiplication: "+(a*b)); 
		        break;
		    case '/':
		         System.out.println("Division: "+(a/b)); 
		        break;
		    case '%':
		         System.out.println(" module: "+(a%b)); 
		        break;
		     default:
		     System.out.println("Invalid Symbol");   
		}
	}
}


OUTPUT:

Enter the two value
37
77
Enter the symbol
*
Multiplication: 2849

````
## 182.Implement a Fibonacci series generator using memoization.
````java[]

package sample;
import java.util.*;
public class Main13 {
public static int fib(int n) {
	if(n==0) {
		return 0;
	}
	if(n==1) {
		return 1;
	}
	
	return fib(n-1)+fib(n-2);
}
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner s=new Scanner(System.in);
		System.out.println("Enter the value of n");
		int n=s.nextInt();
		System.out.println("Fibnacci of number " +n);
	    for(int i=0;i<n;i++) {
	    	int result=fib(i);
	    	System.out.print(result+" ");
	    }

	}

}


OUTPUT:

Enter the value of n
10
Fibnacci of number 10
0 1 1 2 3 5 8 13 21 34 

````
## 183.Create a random password generator.
````java[]
package sample;

import java.util.Random;

public class Main12 {
    public static String generatePassword(int length) {
        String characters = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789!@#$%^&*";
        Random random = new Random();
        StringBuilder password = new StringBuilder();

        for (int i = 0; i < length; i++) {
            int index = random.nextInt(characters.length());
            password.append(characters.charAt(index));
        }

        return password.toString();
    }

    public static void main(String[] args) {
        int length = 8; 
        String password = generatePassword(length);
        System.out.println("Generated Password: " + password);
    }
}

OUTPUT:

Generated Password: &2DHSD0c

````
## 184.Create a simple command-line chat application.
````java[]


````
## 185.Implement a quiz program that uses arrays.
````java[]


````
## 186.Create a program to count words in a sentence.
````java[]

package sample;
import java.util.*;
public class Main10 {

	public static void main(String[] args) {
		Scanner s=new Scanner(System.in);
		System.out.println("Enter the sentence ");
		String str=s.nextLine();
		System.out.println("User input=  " + str);
		if(str.length()==0) {
			System.out.println("Count of the words= 0");
			
		}
		int count=1;
		for(int i=0;i<str.length()-1;i++) {
			if(str.charAt(i)==' ' && str.charAt(i+1)!=' ') {
				count++;
			}
		}
		System.out.println(" Count of the words in the sentence= "+count);

	}

}


OUTPUT:

Enter the sentence 
i will get placed in a good company
User input=  i will get placed in a good company
Count of the words in the sentence= 8

````
## 187.Implement string compression (e.g., "aaabbb" -> "a3b3").

````java[]


````
## 188.Create a program to generate the first N prime numbers.
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
## 189.Create an interactive program to show user details.

````java[]
package sample;
import java.util.*;
public class Main11 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner s=new Scanner(System.in);
		
		System.out.println("Enter your name");
		String name=s.nextLine();
		System.out.println("Enter your age");
		int age=s.nextInt();
		System.out.println("Enter your phone number");
		long number=s.nextLong();
		s.nextLine();
		System.out.println("Enter you city");
		String city=s.nextLine();
		System.out.println("Enter you state");
		String state=s.nextLine();
		System.out.println("Enter you country");
		String country=s.nextLine();
		System.out.println("Enter you email");
		String email=s.nextLine();
		
		System.out.println(" ****USER DETAIL**** ");
		System.out.println("Name: "+ name);
		System.out.println("Age: "+ age);
		System.out.println("Number: "+ number);
		System.out.println("City: "+ city);
		System.out.println("State: "+ state);
		System.out.println("Country: "+ country);
		System.out.println("Email: "+ email);
	}

}


OUTPUT:

Enter your name
Nanthini
Enter your age
20
Enter your phone number
9935365
Enter you city
Madurai
Enter you state
Tamilnadu
Enter you country
India
Enter you email
nan2@gmail.com
 ****USER DETAIL**** 
Name: Nanthini
Age: 20
Number: 9935365
City: Madurai
State: Tamilnadu
Country: India
Email: nan2@gmail.com


````
## 190 .Build a basic database system with file operations.

````java[]


````
## 191.Implement a voting system using classes and loops.
````java[]



````
## 192.Create a program to convert numbers to words.
````java[]



````
## 193 .Build a simple bank account system with balance checking.

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
## 194.Create a dynamic menu-driven program using loops.
````java[]


````
## 195.Implement a Tic-Tac-Toe game with a simple AI.
````java[]

````
## 196. Build a currency converter program.

````java[]



````
## 197.Create a program to count the frequency of words in a sentence.
````java[]


````
## 198.Write a program to find the longest word in a string.
````java[]


````
## 199.Create a simple ATM simulation with deposit/withdraw functions.
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
## 200.Write a program to manage student records.

````java[]



````
