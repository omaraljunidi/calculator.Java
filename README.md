import java.util.Scanner;

public class Calculator {
    public static void main(String[] args) {
        Scanner x = new Scanner(System.in);
        
        System.out.println("Enter a number 1:");
        double number1 = x.nextDouble();
        
        System.out.println("Enter a number 2:");
        double number2 = x.nextDouble();
        
        System.out.println("enter the operation (*,+,/,- ,%):");
        
        char op = x.next().charAt(0); 
        
        switch (op) {
            case '+':
                System.out.println("Result = " + (number1 + number2));
                break;
                
            case '-':
                System.out.println("Result = " + (number1 - number2));
                break;
            //omar aljun07
            case '*':
                System.out.println("Result = " + (number1 * number2));
                break;
                
            case '/':
                if (number2 != 0) {
                    System.out.println("Result = " + (number1 / number2));
                } else {
                    System.out.println("Error: Cannot divide by zero");
                }
                break; 
                //omar aljun07
            default:
                System.out.println("You're stupid, you don't know how to calculate it. ");
        }
    }
