[program-1 for calculator ](#code1)
[program-2 for HelloWorld ](#code2)
[program-3 for Armstrong ](#code3)
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

##assci-3
[
```
class Armstrong {
   Armstrong() {
   }

   void check(int var1) {
      int var3 = 0;

      int var4;
      for(var4 = var1; var1 > 0; var1 /= 10) {
         int var2 = var1 % 10;
         var3 += var2 * var2 * var2;
      }

      if (var3 == var4) {
         System.out.println("Armstrong");
      } else {
         System.out.println("Not Armstrong");
      }

   }

   public static void main(String[] var0) {
      Armstrong var1 = new Armstrong();
      var1.check(153);
   }
}
```
<img width="114" height="28" alt="Screenshot 2026-03-12 222509" src="https://github.com/user-attachments/assets/8bbb59fc-5c65-41f9-a639-ee9f5c2a2792" />
]
#assci-3
