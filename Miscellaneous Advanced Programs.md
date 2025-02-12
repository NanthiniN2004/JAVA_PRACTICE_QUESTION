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


````
## 183.Create a random password generator.
````java[]


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



````
## 189.Create an interactive program to show user details.

````java[]


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


````
## 200.Write a program to manage student records.

````java[]



````
