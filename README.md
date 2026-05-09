# java-calculator-


import java.util.Scanner;

public class practice_56 {
    static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        while (true){

            System.out.println("/n===== Calculator =====");
            System.out.println("1.Addition");
            System.out.println("2.subtration");
            System.out.println("3.Multiplication");
            System.out.println("4.Division");
            System.out.println("5.Exit");


            System.out.println("choose option ");
            int choice = sc.nextInt();


            if (choice == 5) {
                System.out.println("Calculator closed");
                break;
            }

            System.out.println("Enter first number. ");
            double a = sc.nextDouble();

            System.out.println("Enter second number");
            double b = sc.nextDouble();

            double result;

            if (choice == 1) {
                result = a+b;
                System.out.println("Result =" + result);

            } else if (choice == 2) {
                result = a-b;
                System.out.println("Result = " + result);

            } else if (choice == 3) {
                result = a*b;
                System.out.println("Result = " + result );

            } else if (choice == 4) {

                if (b != 0) {
                    result = a / b;
                    System.out.println("Result = "+ result);
                } else {
                    System.out.println("Cannot devide by zero");
                    }

                } else {
                    System.out.println("Invalid choice");
                }
            }
sc.close();

        }
    }