# SimpleCalculator-using-Java
I have created Simple Calculator using java basics like loop,contional,scanner.


import java.util.Scanner;


public class SimpleCalculator {
  public static void main(String[]args) {
	  Scanner  sc=new Scanner(System.in);
	  while(true)
	  {
	  System.out.println("Simple Calculator");
	  System.out.println("Enter\n + for Addition\n - for Subtraction\n * for Multiplication\n / for Division");
	  String input=sc.next(); 
	  System.out.println("Enter First Number:");
	  int Num1 = sc.nextInt();
	  System.out.println("Enter Second Number:");
	  int Num2 = sc.nextInt();
	  
	  switch(input) {
	  case "+":System.out.println("Addition:"+(Num1+Num2));
	       break;
	  case "-":System.out.println("Subtraction:"+(Num1-Num2));
           break;
	  case "*":System.out.println("Multiplication:"+(Num1*Num2));
           break;
	  case "/":
		  if(Num2==0) {
			  System.out.println("Cannot divide by Zero");
		  }
		  else {
		  System.out.println("Division:"+(Num1/Num2));
		  }
           break;
      default:
    	  System.out.println("Enter the Correct option");
	  }
	  System.out.println("Enter Y to Continue N to Exit");
	  String input2 = sc.next();
	  if (input2.equals("y") || input2.equals("Y"))
		  continue;
	  else
		  break;
	  }
  }
}
