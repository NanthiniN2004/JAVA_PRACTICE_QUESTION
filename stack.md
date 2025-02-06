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

## 

````java[]

import java.util.*;
class Stack{
    int top1;
    int top2;
    int size;
    int[] a;
   public  Stack(int size){
     top1=-1;
     top2=size;
    a=new int[size];
    }
    public void push1(int data){
    if(top1<top2-1){
    top1++;
    a[top1]=data;
    }
    else{
    System.out.println("Stack full");
    }
    }
     
     public void push2(int data){
    if(top1<top2-1){
    top2--;
    a[top2]=data;
    }
    else{
    System.out.println("Stack full");
    }
    }
    public int pop1(){
        if(top1>=0){
           return  a[top1--];
        }
        else{
        System.out.println("stack empty");
        return -1;
    }
    }
    public int pop2(){
        if(top2 < size){
            return a[top2++];
        }
        else{
        System.out.println("stack empty");
        return -1;
    }
    }
    public void peek(){
        if(top1==-1){
            System.out.println("stack empty");
        }
        else{
            System.out.println(a[top1]);
        }
    }
   
    public void display1(){
        System.out.println("stack1");
        for(int i=top1;i>=0;i--){
            System.out.print(a[i]+" ");
        }
    }
    
      public void display2(){
          System.out.println("stack2");
        for(int i=top2;i<=size;i++){
            System.out.print(a[i]+" ");
        }
    }
    
}

public class Main{
    public static void main(String args[]){
        Scanner s=new Scanner(System.in);
        System.out.println("Enter the size of the stack");
        int size=s.nextInt();
        System.out.println("Enter the element you want to push in first stack");
        int n1=s.nextInt();
        System.out.println("Enter the element you want to push in Second stack");
        int n2=s.nextInt();
        
        Stack obj=new Stack(size);
        System.out.println("Enter the element");
        for(int i=0;i<n1;i++){
            int val=s.nextInt();
            obj.push1(val);
        }
         System.out.println("Enter the element");
        for(int i=0;i<n2;i++){
            int val1=s.nextInt();
            obj.push2(val1);
        }
        System.out.println("Before popping:");
        obj.display1();
        obj.display2();

        System.out.println("Popping from Stack 1 → " + obj.pop1());
        System.out.println("Popping from Stack 2 → " + obj.pop2());


        System.out.println("After popping:");
        obj.display1();
        obj.display2();

        
        
    }
}
