## 161.Create a simple text-based game using if-else and loops. 
````java[]

package Nanthu;

import java.util.*;

public class Main7 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("Welcome to the Haunted House!");
        System.out.println("You are standing in front of a creepy old house. Do you enter? (yes/no)");
        
        String choice = scanner.nextLine();
        
        if (choice.equalsIgnoreCase("yes")) {
            System.out.println("You step inside and the door creaks shut behind you.");
            System.out.println("You see two doors: one on the left and one on the right. Which one do you choose? (left/right)");
            
            choice = scanner.nextLine();
            
            if (choice.equalsIgnoreCase("left")) {
                System.out.println("You enter a dark room and suddenly hear whispers. You feel a chill down your spine.");
                System.out.println("You found a hidden treasure! You win!");
            } else if (choice.equalsIgnoreCase("right")) {
                System.out.println("You walk into a dimly lit hallway. A ghostly figure appears and chases you out of the house.");
                System.out.println("You barely escape with your life. Game over!");
            } else {
                System.out.println("Invalid choice. The house consumes you. Game over!");
            }
        } else if (choice.equalsIgnoreCase("no")) {
            System.out.println("You decide not to enter and walk away safely. Maybe next time!");
        } else {
            System.out.println("Invalid choice. The house consumes you. Game over!");
        }
        
        scanner.close();
    }
}

OUTPUT:

Welcome to the Haunted House!
You are standing in front of a creepy old house. Do you enter? (yes/no)
yes
You step inside and the door creaks shut behind you.
You see two doors: one on the left and one on the right. Which one do you choose? (left/right)
left
You enter a dark room and suddenly hear whispers. You feel a chill down your spine.
You found a hidden treasure! You win!


````
## 162 .Build a password validation program with loops and conditions. 
````java[]



````
## 163.Implement a Tic-Tac-Toe game using loops and conditions. 
````java[]



`````
## 164.Implement a simple file I/O program. 
````java[]



`````
## 165.Create a phonebook program with search functionality. 

````java[]




````
## 166.Implement a ticket booking system with class and objects. 

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
## 167.Create a random number generator for a guessing game. 
````java[]

package Nanthu;
import java.util.*;
public class Main2 {

	public static void main(String[] args) {
		Scanner s=new Scanner(System.in);
		Random random=new Random();
		
		int numberToGuess=random.nextInt(100)+1;
		int attempt=0;
		int userinput=0;
		System.out.println("  WELCOME TO NUMBER GUESSING GAME  ");
		System.out.println("  GUESS A NUMBER BETWEEN 1 AND 100 ");
		while(numberToGuess != userinput) {
			 System.out.println("Enter the Guess");
			 userinput=s.nextInt();
			 attempt++;
			 
			 if(userinput < numberToGuess)
			 {
				 System.out.println("To low! Try Again");
			 }
			 else if(userinput> numberToGuess) {
				 System.out.println("To high! Try Again");
			 }
			 else {
				 System.out.println("Congratulations! You guessed the number in " + attempt + " attempts.");
			 }
		}

	}

}

OUTPUT:

 WELCOME TO NUMBER GUESSING GAME  
  GUESS A NUMBER BETWEEN 1 AND 100 
Enter the Guess
55
To low! Try Again
Enter the Guess
71
To high! Try Again
Enter the Guess
60
To high! Try Again
Enter the Guess
58
To low! Try Again
Enter the Guess
59
Congratulations! You guessed the number in 5 attempts.


````
## 168 .Build a simple calendar program using loops. 
````java[]

package Nanthu;
import java.util.*;

public class Main9 {

    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);
        System.out.println("Total number of days in the month:");
        int totalday = s.nextInt();
        System.out.println("Enter the starting day of the week (1 for Monday, 7 for Sunday):");
        int start = s.nextInt();
        
        System.out.println("\n  Mon  Tue  Wed  Thu  Fri  Sat  Sun ");
        
        int day = 1;
        int current = start - 1; 
        
        
        for (int i = 0; i < current; i++) {
            System.out.print("     "); 
        }
        
        
        for (int i = current; day <= totalday; i++) {
            System.out.printf("%4d ", day);
            if ((i + 1) % 7 == 0 || day == totalday) {
                System.out.println(); 
            }
            day++;
        }
    }
}

OUTPUT:

Total number of days in the month:
30
Enter the starting day of the week (1 for Monday, 7 for Sunday):
1

  Mon  Tue  Wed  Thu  Fri  Sat  Sun 
   1    2    3    4    5    6    7 
   8    9   10   11   12   13   14 
  15   16   17   18   19   20   21 
  22   23   24   25   26   27   28 
  29   30 



`````
## 169.Create a program that checks for valid email addresses. 
`````java[]

package Nanthu;
import java.util.*;
import java.util.regex.Pattern;
public class Main10 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner s=new Scanner(System.in);
		System.out.println("Enter the Email");
		String email=s.nextLine();
		if(isValid(email)) {
			System.out.println(" Valid Email Address");
		}
		else {
			System.out.println("Not valid Email Address");
		}

	}
	public static boolean isValid(String email) {
		String emailRegex = "^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\\.[a-zA-Z]{2,}$";
		return Pattern.matches(emailRegex, email);
	}

}


OUTPUT:
Enter the Email
nanthini@gmail.com
 Valid Email Address



`````
## 170 .Build a number encryption/decryption program. 
````java[]




`````


## 171.Create a weather app interface using control statements.
````java[]

package sample;

import java.util.Scanner;

public class Main6 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("Welcome to the Weather App!");
        System.out.println("Enter the current temperature (°C):");
        int temperature = scanner.nextInt();

        System.out.println("Is it raining? (yes/no):");
        String rainInput = scanner.next().toLowerCase();
        boolean isRaining = rainInput.equals("yes");

        System.out.println("Is it windy? (yes/no):");
        String windInput = scanner.next().toLowerCase();
        boolean isWindy = windInput.equals("yes");

        System.out.println("Choose the city: ");
        System.out.println("1. New York\n2. London\n3. Tokyo\n4. Sydney");
        int cityChoice = scanner.nextInt();
        String city = "";

        switch (cityChoice) {
            case 1: city = "New York"; break;
            case 2: city = "London"; break;
            case 3: city = "Tokyo"; break;
            case 4: city = "Sydney"; break;
            default: city = "Unknown City";
        }

        System.out.println("\nWeather Report for " + city + ":");
        
        if (temperature > 30) {
            System.out.println("It's very hot outside! Stay hydrated.");
        } else if (temperature > 20) {
            System.out.println("It's warm outside. Enjoy your day!");
        } else if (temperature > 10) {
            System.out.println("It's cool outside. A light jacket is recommended.");
        } else {
            System.out.println("It's cold outside! Wear warm clothes.");
        }

        if (isRaining) {
            System.out.println("It's raining. Don't forget your umbrella!");
        }

        if (isWindy) {
            System.out.println("It's windy. Be cautious if you're going outside.");
        }

        System.out.println("\nThank you for using the Weather App!");
        scanner.close();
    }
}


output:

Welcome to the Weather App!
Enter the current temperature (°C):
40
Is it raining? (yes/no):
no
Is it windy? (yes/no):
yes
Choose the city: 
1. New York
2. London
3. Tokyo
4. Sydney
2

Weather Report for London:
It's very hot outside! Stay hydrated.
It's windy. Be cautious if you're going outside.

Thank you for using the Weather App!


````
## 172.Write a program for bubble sort.
````java[]


import java.util.*;
public class Main
{
	public static void main(String[] args) {
	   Scanner s=new Scanner(System.in);
		int n=s.nextInt();
		int[] a=new int[n];
		for(int i=0;i<n;i++){
		    a[i]=s.nextInt();
		}
		bubblesort(a,n);
			for(int i=0;i<n;i++){
		    System.out.print(a[i]+" ");
		}
		
	}
	public static void bubblesort(int[] a,int n){
		for(int i=0;i<n;i++){
		    for(int j=i;j<n-1-i;j++){
		        if(a[j]>a[j+1]){
		            int temp=a[j];
		            a[j]=a[j+1];
		            a[j+1]=temp;
		        }
		    }
		}
	
	}
}


OUTPUT:

5
3
1
5
2
4
1 2 3 4 5


````
## 173.Implement insertion sort using loops.
````java[]

package sample;
import java.util.*;
public class Main4 {
 public static void insertionSort(int a[],int n) {
	 for(int i=0;i<=n-2;i++) {
		 for(int j=i+1;j>0;j--) {
			 if(a[j] <a[j-1]) {
				 int temp=a[j];
				 a[j]=a[j-1];
				 a[j-1]=temp;
			 }
			 else {
				 break;
			 }
		 }
	 }
 }
	public static void main(String[] args) {
		Scanner s=new Scanner(System.in);
		System.out.println("Enter the size of the array");
		int n=s.nextInt();
		int a[]=new int[n];
		System.out.println("Enter the element");
		for(int i=0;i<n;i++) {
			a[i]=s.nextInt();
		}
		System.out.println("After sorting");
		insertionSort(a,n);
		for(int i:a) {
			System.out.print(i+" ");
		}

	}

}


OUTPUT:

Enter the size of the array
5
Enter the element
8
3
5
9
1
After sorting
1 3 5 8 9 


````
## 174.Perform quicksort on an array using recursion.

````java[]

package sample;

import java.util.*;


public class Main7 {
   public static void main(String[] args) {
       Scanner s=new Scanner(System.in);
       System.out.println("Enter the size of the array");
		int n=s.nextInt();
		int array[]=new int[n];
		System.out.println("Enter the element");
		for(int i=0;i<n;i++) {
			array[i]=s.nextInt();
		}
       System.out.println("Unsorted Array: " + Arrays.toString(array));
       quickSort(array, 0, array.length - 1);
       System.out.println("  Sorted Array: " + Arrays.toString(array));

   }
   public static void quickSort(int[] arr, int low, int high) {
       if (low < high) {
           int pi = partition(arr, low, high);
           quickSort(arr, low, pi - 1);
           quickSort(arr, pi + 1, high);
       }
   }

   private static int partition(int[] arr, int low, int high) {
       int pivot = arr[high];
       int i = (low - 1);
       for (int j = low; j < high; j++) {
           if (arr[j] < pivot) {
               i++;
               int temp = arr[i];
               arr[i] = arr[j];
               arr[j] = temp;
           }
       }
       int temp = arr[i + 1];
       arr[i + 1] = arr[high];
       arr[high] = temp;

       return i + 1;	   
   }
}

OUTPUT:

Enter the size of the array
6
Enter the element
8
2
5
4
12
3
Unsorted Array: [8, 2, 5, 4, 12, 3]
  Sorted Array: [2, 3, 4, 5, 8, 12]


````
## 175.Implement selection sort with a loop.
````java[]

package sample;
import java.util.*;
public class Main5 {
	public static void selectionSort(int a[],int n) {
		for(int i=0;i<n-1;i++) {
			int midindex=i;
			for(int j=i+1;j<n;j++) {
				if(a[j]<a[midindex]) {
					midindex=j;
				}
			}
			int temp=a[midindex];
			a[midindex]=a[i];
			a[i]=temp;
		}
	}

	public static void main(String[] args) {
		Scanner s=new Scanner(System.in);
		System.out.println("Enter the size of the array");
		int n=s.nextInt();
		int a[]=new int[n];
		System.out.println("Enter the element");
		for(int i=0;i<n;i++) {
			a[i]=s.nextInt();
		}
		System.out.println("After sorting");
		selectionSort(a,n);
		for(int i:a) {
			System.out.print(i+" ");
		}

	}

}


OUTPUT:

Enter the size of the array
5
Enter the element
71
77
51
55
11
After sorting
11 51 55 71 77 


````
## 176.Perform a binary search recursively.
````java[]

package sample;
import java.util.*;
public class Main1 {
 public static int binarySearch(int[] a,int start,int end,int target)
 {
	 while(start<end) {
		 int mid=(start+end)/2;
		 if(a[mid]==target) {
			 return mid;
		 }
		 else if(a[mid]>target) {
			 return binarySearch(a,start,mid-1,target);
		 }
		 else {
			 return binarySearch(a,mid+1,end,target);
		 }
	 }
	 return -1;
 }
	public static void main(String[] args) {
     Scanner s=new Scanner(System.in);
     System.out.println("Enter the size of the array");
     int n=s.nextInt();
     int[] a=new int[n];
     System.out.println("Ënter the array element");
     for(int i=0;i<n;i++) {
    	 a[i]=s.nextInt();
     }
     System.out.println("Enter the target element");
     int target=s.nextInt();
     int result=binarySearch(a,0,n-1,target);
     if(result==-1) {
    	 System.out.println("Element is not found");
     }
     else {
    	System.out.println(" Element is found "+ result);
     }

	}

}
OUTPUT:

Enter the size of the array
5
Ënter the array element
10
20
30
40
50
Enter the target element
40
Element is found 3


````
## 177.Create a class to manage a simple bank account.

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
## 178.Write a program for linear search recursively.
````java[]

package sample;
import java.util.*;

public class Main2 {
	public static int linearSearch(int[] a,int n,int target) {
		if(n==0) {
			return 0;
		}
		else if(a[n-1]==target) {
			return n-1;
		}
		return linearSearch(a,n-1,target);
	}
public static void main(String args[]) {
	Scanner s=new Scanner(System.in);
    System.out.println("Enter the size of the array");
    int n=s.nextInt();
    int[] a=new int[n];
    System.out.println("Ënter the array element");
    for(int i=0;i<n;i++) {
   	 a[i]=s.nextInt();
    }
    System.out.println("Enter the target element");
    int target=s.nextInt();
    int result=linearSearch(a,n,target);
    if(result==-1) {
    	System.out.println(" Element Not found");
    }
    else {
    	 System.out.println(
                 "The element " + target + " is found at "
                 +result + " index of the given array.");
    }
}
}


OUTPUT:

Enter the size of the array
5
Ënter the array element
90
50
71
55
101
Enter the target element
50
The element 50 is found at 1 index of the given array.


````
## 179.Implement depth-first search using a stack.

````java[]



````
## 180.Implement breadth-first search using a queue.
````java[]



````
