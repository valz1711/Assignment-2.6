1)
  import java.util.ArrayList;
  import java.util.Collections;
  import java.util.Scanner;
  public class acad {
    public static void main(String[] args) {
      Scanner ss = new Scanner(System.in);
      int a=ss.nextInt();//Input the first number
      int b=ss.nextInt();//Input the second number
      ArrayList<Integer> even = new ArrayList<Integer>();//to store the even numbers as we don't no the range
      ArrayList<Integer> odd = new ArrayList<Integer>();//to store the odd numbers as we don't no the range
      for(int i=a;i<=b;i++) //for the given range
      {
          if(i%2==0)//condition for even
          {
              even.add(i);
          }
          else
          {
              odd.add(i);
          }
      }
      System.out.println("Even Numbers are:");
      Collections.sort(even);
      System.out.println(even);//display even numbers
      System.out.println("Odd Numbers are:");
      Collections.sort(odd);//display odd numbers
      System.out.println(odd);
      ss.close();
    }
   }
  
2)
  import java.util.ArrayList;
  import java.util.Collections;
  import java.util.Scanner;
  public class acad {
    public static void main(String[] args) {
      Scanner ss = new Scanner(System.in);
      int a=ss.nextInt();//Input the number to get the first 10 multiples 
      int mul[] = new int[10];//to store result
      for(int i=0;i<10;i++)   //for the given range
      {
          mul[i] = a*(i+1);
      }
      System.out.println("Multiple of the entered numbers:");
      for(int j=0;j<10;j++)// to display the first 10 multiples
      {
          System.out.println(mul[j]);
      }
      ss.close();
      }
    }
 
3)
import java.util.*;
public class acad {
  public static void main(String[] args) {
      Scanner ss = new Scanner(System.in);
      int a=ss.nextInt(); //Input number
      int b=ss.nextInt(); //Input number
      int d =ss.nextInt(); //Input number
      sum(a,b); //method called with two variables
      sum(a,b,d); //method called with three variables
      ss.close();
      }
  static void sum(int a,int b) //method to add two variables
  {
    int c;
    c=a+b;
    System.out.println("Method with two variables");
    System.out.println(c); //print the result
   }
  static void sum(int a,int b,int d)//method to multiply two variable and add third
  {
      int c;
      c=a*b+d;
      System.out.println("Method with two variables"+"\n"+c);//print the result
   }
  }
