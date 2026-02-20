## assci-1
[
```
import java.util.Scanner;

public class calculator {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter first number: ");
        int a = sc.nextInt();

        System.out.print("Enter second number: ");
        int b = sc.nextInt();

        add(a, b);
        sub(a, b);
        mul(a, b);
        div(a, b);

        sc.close();
    }

    public static void add(int a, int b) {
        System.out.println("Addition: " + (a + b));
    }

    public static void sub(int a, int b) {
        System.out.println("Subtraction: " + (a - b));
    }

    public static void mul(int a, int b) {
        System.out.println("Multiplication: " + (a * b));
    }

    public static void div(int a, int b) {
        if (b == 0) {
            System.out.println("Division: Cannot divide by zero");
        } else {
            System.out.println("Division: " + (a / b));
        }
    }
}
```
<img width="460" height="171" alt="image" src="https://github.com/user-attachments/assets/325a9760-76f6-4275-bd1e-f13b3712e510" />
]
#assci-1

## assci-2
[
```
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```
<img width="138" height="38" alt="image" src="https://github.com/user-attachments/assets/36572a87-731d-4a6e-b18e-9ab856a6f314" />
]
#assci-2
