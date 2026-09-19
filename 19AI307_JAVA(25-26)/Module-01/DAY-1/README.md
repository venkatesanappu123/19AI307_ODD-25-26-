# Ex.No:1(A) INTRODUCTION TO JAVA PROGRAMMING, DATA TYPES, VARIABLES AND OPERATORS

## QUESTION:
Lovely is a treasure hunter and has reached the final chamber of the dungeon. To unlock the treasure chest, she must enter a secret 4-digit code.

A riddle appears on the wall:

"The code is hidden in the numbers you enter. Solve these puzzles to form it!"

The puzzle has 4 steps:

First digit = sum of the first two numbers

Second digit = difference between the third and fourth numbers

Third digit = product of the second and fourth numbers

Fourth digit = remainder when third number is divided by first number

Input Format:
Enter four numbers as input (integers):

<number1>
<number2>
<number3>
<number4>
Output Format:

The treasure code
The treasure code is: <digit1><digit2><digit3><digit4>

## AIM:
To write a Java program that reads four integer inputs from the user, performs arithmetic operations (addition, subtraction, multiplication, and modulus), and combines the results to display a treasure code.

## ALGORITHM :
1.	Start the program and create a Scanner object.
2.	Read four integer inputs from the user.
3.	Compute digit1, digit2, digit3, and digit4 using +, -, *, and % operations.
4.	Concatenate and print the treasure code.
5.	Stop the program.

## PROGRAM:

### Program to Implement Variables and Operators Using Java

**Developed by:** VENKATESAN R

**Register Number:** 212224230299


### Sourcecode.java:
```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int number1 = Integer.parseInt(scanner.nextLine());
        int number2 = Integer.parseInt(scanner.nextLine());
        int number3 = Integer.parseInt(scanner.nextLine());
        int number4 = Integer.parseInt(scanner.nextLine());

        int digit1 = number1 + number2;
        int digit2 = number3 - number4;
        int digit3 = number2 * number4;
        int digit4 = number3 % number1;

        System.out.println("The treasure code is: " + digit1 + "" + digit2 + "" + digit3 + "" + digit4);

        scanner.close();
    }
}
```






## OUTPUT:
<img width="1158" height="518" alt="image" src="https://github.com/user-attachments/assets/c58c4aea-a5d2-4032-afb3-dc765bd0f33b" />


## RESULT:
Thus, the Java program to generate a treasure code using arithmetic operations on four user inputs was successfully executed and the output was verified.




