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
