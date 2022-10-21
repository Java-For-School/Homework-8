# Homework 8 22/10/2022

#### Solutions:
##### Problem 1:

```java
import java.util.Scanner;

class HelloWorld {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        int number = scanner.nextInt();
        System.out.println("The selected number is: " + number);
        System.out.println("Your number factorial: " + getFactorial(number, 1));
        
        
    }
    public static int getFactorial(int number, int current) {
        if (number == 0) return current;
        return getFactorial(number - 1, number * current);
    }
}
```
##### Problem 2:

```java
import java.util.Scanner;

class HelloWorld {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        boolean flag = true;
        int input, sum = 0, inputCount = 0;
        
        
        while(flag) {
            input = scanner.nextInt();
            if (input == -1) { flag = false; break; }
            inputCount++;
            sum += input;
        }
        
        System.out.println("You have been gifted an average of: " + sum / inputCount + " per attendee of your wedding.");
        
    }
   
}
```
