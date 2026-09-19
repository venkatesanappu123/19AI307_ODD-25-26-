# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
The much-anticipated "Publishers Federation Book Expo" has returned, promising an even grander experience with nearly a million books on display. This year, the event is being hosted on the topmost floor—floor number N—of the prestigious Hotel Grand Regency.

Williams, a passionate book enthusiast, arrives at the expo and is now looking for the fastest way to reach the ground floor from the N-th floor. He has two options: take the stairs or use the elevator.

The stairs are built at a 45-degree angle, and Williams can descend them at a speed of V1 meters per second. Alternatively, the elevator always starts at the ground floor, travels up to the N-th floor to pick him up (the pickup is instantaneous), and then descends back to the ground floor at a speed of V2 meters per second.

The total vertical distance the elevator travels in one complete trip (up and down) is 2 × N meters. Meanwhile, the stairs span a diagonal length of √2 × N meters due to the 45-degree incline.

Your task is to help Williams choose the faster route. Based on the time it would take using either method, determine whether Stairs or Elevator is the better option.

Input :
N, V1, and V2 (Follow the same order).

Output :
Stairs if taking the stairs is faster, or Elevator if the elevator is the quicker option.



## AIM:
To write a Java program that determines whether using stairs or an elevator is faster based on given speeds and distance.

## ALGORITHM :
1.	Start the program and create a Scanner object.
2. Read three integer inputs — n, v1, and v2.
3. Calculate elevatorTime = (2 × n) / v2 and stairsTime = (√2 × n) / v1.
4. Compare both times and print "Stairs" if stairs are faster, else "Elevator".
5. End the program.





## PROGRAM:
### Program to Implement Variables and Operators Using Java

**Developed by:** ASWIN B

**Register Number:** 212224110007

### SOURCE CODE:
```java
import java.util.Scanner;

public class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        int n = sc.nextInt();
        int v1 = sc.nextInt();
        int v2 = sc.nextInt();

        double elevatorDistance = 2.0 * n;
        double elevatorTime = elevatorDistance / v2;

        double stairsDistance = Math.sqrt(2) * n;
        double stairsTime = stairsDistance / v1;

        if (stairsTime < elevatorTime) {
            System.out.println("Stairs");
        } else {
            System.out.println("Elevator");
        }

        sc.close();
    }
}
```

## OUTPUT:
<img width="1151" height="347" alt="image" src="https://github.com/user-attachments/assets/ff0cc3d1-fa02-488b-a30c-bcb7d013aa07"/>


## RESULT:
The program successfully determines the faster option between stairs and elevator.




