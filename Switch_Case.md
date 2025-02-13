## 41.Implement a simple calculator using switch case.
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
## 42.Convert a number to its word equivalent (1 to 10) using switch.
````java[]


package Nanthu;
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the value(1 to 10)");
	    int n=s.nextInt();

		switch(n){
		    case 1:
		        System.out.println("ONE");
		        break;
		     case 2:
		    	  System.out.println("TWO");
		        break;        
		    case 3:
		    	  System.out.println("THREE");
		        break;
		    case 4:
		    	  System.out.println("FOUR");
		        break;
		      case 5:
		            System.out.println("FIVE");
		         break;
		      case 6:
		            System.out.println("SIX");
		         break;
		      case 7:
		            System.out.println("SEVEN");
		         break;
		      case 8:
		            System.out.println("EIGHT");
		         break;
		      case 9:
		            System.out.println("NINE");
		         break;
		      case 10:
		            System.out.println("TEN");
		         break;
		        
		     default:
		     System.out.println("Invalid Option");   
		}
	}
}

OUTPUT:

Enter the value(1 to 10)
5
FIVE

````
## 43.Find the day of the week using switch statement.
````java[]


package Nanthu;
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the DAY(1 to 7)");
	    int n=s.nextInt();

		switch(n){
		    case 1:
		        System.out.println("SUNDAY");
		        break;
		     case 2:
		    	  System.out.println("MONDAY");
		        break;        
		    case 3:
		    	  System.out.println("TUESDAY");
		        break;
		    case 4:
		    	  System.out.println("WEDNESDAY");
		        break;
		    case 5:
	            System.out.println("THURSDAY");
	         break;
		      case 6:
		            System.out.println("FRIDAY");
		         break;
		      case 7:
		            System.out.println("SATURDAY");
		         break;
		     
		        
		     default:
		     System.out.println("Invalid Option");   
		}
	}
}

output:

Enter the DAY(1 to 7)
7
SATURDAY


````
## 44.Convert a number to its Roman numeral equivalent using switch. 
````java[]

package Nanthu;
import java.util.*;
public class Main1
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the value(1 to 10)");
	    int n=s.nextInt();

		switch(n){
		    case 1:
		        System.out.println("I");
		        break;
		     case 2:
		    	  System.out.println("II");
		        break;        
		    case 3:
		    	  System.out.println("III");
		        break;
		    case 4:
		    	  System.out.println("IV");
		        break;
		      case 5:
		            System.out.println("V");
		         break;
		      case 6:
		            System.out.println("VI");
		         break;
		      case 7:
		            System.out.println("VII");
		         break;
		      case 8:
		    	  System.out.println("VIII");
			         break;
			      case 9:
			            System.out.println("IX");
			         break;
			      case 10:
			            System.out.println("X");
			         break;
			        
			     default:
			     System.out.println("Invalid Option");   
			}
		}
	}


output:

Enter the value(1 to 10)
6
VI

````
## 45.Implement a basic menu-driven program using switch-case.
````java[]



````
## 46.Print all numbers from 1 to n in reverse using switch.
````java[]


````
## 47.Grade student marks using a switch-case statement.
````java[]

package Nanthu;

import java.util.*;
public class Main3
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the your mark");
	    int mark=s.nextInt();
	    int n=mark/10;

		switch(n){
		case 10:
		    case 9:
		        System.out.println(" Grade A");
		        break;
		     case 8:
		    	  System.out.println("Grade B");
		        break;        
		    case 7:
		    	  System.out.println("Grade C");
		        break;
		    case 6:
		    	  System.out.println("Grade D");
		        break;
		      case 5:
		            System.out.println("Grade E");
		         break;
			        
			     default:
			    	 if(mark>=0 && mark<50) {
			    		 System.out.println("Fail");
			    		 
			    	 }
			    	 else {
			     System.out.println("Invalid Option"); 
			    	 }
			}
		}
	}


OUTPUT:

Enter the your mark
85
Grade B

````
## 48.Perform simple arithmetic operations using switch.

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
## 49.Convert temperature from Celsius to Fahrenheit or vice versa using switch.

````java[]


````
## 50.Find the number of days in a month using switch-case.
````java[]
package Nanthu;
import java.util.*;
public class Main2
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    System.out.println("Enter the Month");
	    String month=s.nextLine();

		switch(month){
		    case "January":
		        System.out.println("31");
		        break;
		     case "February":
		    	  System.out.println("28 or 29");
		        break;        
		    case "March":
		    	  System.out.println("31");
		        break;
		    case "April":
		    	  System.out.println("30");
		        break;
		      case "May":
		            System.out.println("31");
		         break;
		      case "June":
		            System.out.println("30");
		         break;
		      case "July":
		            System.out.println("31");
		         break;
		      case "August":
		            System.out.println("31");
		         break;
		      case "September":
		            System.out.println("30");
		         break;
		      case "October":
		            System.out.println("31");
		         break;
		      case "November":
		            System.out.println("30");
		         break;
		      case "December":
		            System.out.println("31");
		         break;
		         
		     default:
		     System.out.println("Invalid Option");   
		}
	}
}

OUTPUT:

Enter the Month
November
30


````
## 51.Implement a simple banking system with switch-case.

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
## 52.Determine the month name based on its number using switch-case.

````java[]



````
## 53.Calculate the area of different shapes using switch-case.

````java[]


````

## 54.Implement a basic calculator with multiple operations.
````java[]


````
## 55.Determine if a given character is a vowel or consonant using switch-case.

````java[]



````
## 56.Implement a simple menu system for shopping.

````java[]



````
## 57.Convert a time duration in minutes to hours and minutes.
````java[]



````
## 58.Implement a number to word converter (1-10) using switch.
````java[]


````
## 59.Implement a traffic light system using switch.
````java[]


````
## 60.Solve a quadratic equation using switch-case for the discriminant.
````java[]



````
