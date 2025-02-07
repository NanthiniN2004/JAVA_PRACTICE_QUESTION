##  DELETE MIDDLE ELEMENT OF A STACK

````java[]

import java.util.*;
class Stack{
    int top;
    int[] a;
   public  Stack(int size){
     top=-1;
    a=new int[size];
    }
    public void push(int data){
    if(top==a.length-1){
        System.out.println("Stack full");
    }
    top++;
    a[top]=data;
    }
    public int pop(){
        if(top==-1){
            System.out.println("stack empty");
        }
        return a[top--];
    }
    public void peek(){
        if(top==-1){
            System.out.println("stack empty");
        }
        else{
            System.out.println(a[top]);
        }
    }
    public void deleteMiddle(){
    
        int mid=top/2;
        int[] temp=new int[mid];
        for(int i=0;i<mid;i++){
            temp[i]=pop();
        }
        pop();
        for(int i=mid-1;i>=0;i--){
            push(temp[i]);
        }
    }
    public void display(){
        for(int i=top;i>=0;i--){
            System.out.print(a[i]+" ");
        }
    }
}

public class Main{
    public static void main(String args[]){
        Scanner s=new Scanner(System.in);
        System.out.println("Enter the size of the stack");
        int size=s.nextInt();
        System.out.println("Enter the element you want to push");
        int n=s.nextInt();
        Stack obj=new Stack(size);
        System.out.println("Enter the element");
        for(int i=0;i<n;i++){
            int val=s.nextInt();
            obj.push(val);
        }
        System.out.println("before Delete the element");
        obj.display();
        obj.deleteMiddle();
        System.out.println("After delete the element");
        obj.display();
        
    }
}

OUTPUT:

Enter the size of the stack
7
Enter the element you want to push
5
Enter the element
10
20
30
40
50
before Delete the element
50 40 30 20 10 After delete the element
50 40 20 10

````

## TWO STACK IN ONE ARRAY

````java[]



import java.util.*;

class Stack {
    int top1, top2, size;
    int[] a;


    public Stack(int size) {
        this.size = size;
        top1 = -1;     
        top2 = size;    
        a = new int[size];
    }

    public void push1(int data) {
        if (top1 < top2 - 1) {
            a[++top1] = data;
        } else {
            System.out.println("Stack 1 Overflow!");
        }
    }

   
    public void push2(int data) {
        if (top1 < top2 - 1) {
            a[--top2] = data;
        } else {
            System.out.println("Stack 2 Overflow!");
        }
    }


    public int pop1() {
        if (top1 >= 0) {
            return a[top1--];
        } else {
            System.out.println("Stack 1 Underflow!");
            return -1;
        }
    }

    public int pop2() {
        if (top2 < size) {  // FIXED: Check if top2 has moved
            return a[top2++];
        } else {
            System.out.println("Stack 2 Underflow!");
            return -1;
        }
    }

  
    public void peek(int stackNumber) {
        if (stackNumber == 1) {
            if (top1 == -1) {
                System.out.println("Stack 1 is empty");
            } else {
                System.out.println("Top of Stack 1: " + a[top1]);
            }
        } else if (stackNumber == 2) {
            if (top2 == size) {
                System.out.println("Stack 2 is empty");
            } else {
                System.out.println("Top of Stack 2: " + a[top2]);
            }
        }
    }

    public void display1() {
        System.out.println("Stack 1:");
        for (int i = top1; i >= 0; i--) {
            System.out.print(a[i] + " ");
        }
        System.out.println();
    }

    
    public void display2() {
        System.out.println("Stack 2:");
        for (int i = top2; i < size; i++) {  
            System.out.print(a[i] + " ");
        }
        System.out.println();
    }
}


public class Main {
    public static void main(String args[]) {
        Scanner s = new Scanner(System.in);
        System.out.println("Enter the size of the stack:");
        int size = s.nextInt();

        Stack obj = new Stack(size);


        System.out.println("Enter the number of elements for Stack 1:");
        int n1 = s.nextInt();
        System.out.println("Enter elements for Stack 1:");
        for (int i = 0; i < n1; i++) {
            obj.push1(s.nextInt());
        }

        System.out.println("Enter the number of elements for Stack 2:");
        int n2 = s.nextInt();
        System.out.println("Enter elements for Stack 2:");
        for (int i = 0; i < n2; i++) {
            obj.push2(s.nextInt());
        }

        System.out.println("Before popping:");
        obj.display1();
        obj.display2();

      
        obj.peek(1);
        obj.peek(2);

        System.out.println("Popping from Stack 1 → " + obj.pop1());
        System.out.println("Popping from Stack 2 → " + obj.pop2());

     
        System.out.println("After popping:");
        obj.display1();
        obj.display2();

        s.close();
    }
}


output:

Enter the size of the stack:
6
Enter the number of elements for Stack 1:
3
Enter elements for Stack 1:
1
2
3
Enter the number of elements for Stack 2:
3
Enter elements for Stack 2:
4
5
6
Before popping:
Stack 1:
3 2 1 
Stack 2:
6 5 4 
Top of Stack 1: 3
Top of Stack 2: 6
Popping from Stack 1 → 3
Popping from Stack 2 → 6
After popping:
Stack 1:
2 1 
Stack 2:
5 4 


````


