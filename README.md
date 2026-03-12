[program-1 for calculator ](#code1)
[program-2 for HelloWorld ](#code2)
[program-3 for Armstrong ](#code3)
[program-4 for Distance1 ](#code4)
[program-5 for Distance2 ](#code5)
[program-6 for Factorial ](#code6)
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

## assci-3
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

## assci-4
[
```
class Distance1 {
    int km, m, cm;

    void input(int km, int m, int cm) {
        this.km = km;
        this.m = m;
        this.cm = cm;
    }

    void add(Distance1 d1, Distance1 d2) {
        cm = d1.cm + d2.cm;
        m = d1.m + d2.m + cm / 100;
        cm = cm % 100;
        km = d1.km + d2.km + m / 1000;
        m = m % 1000;
    }

    void display() {
        System.out.println(km + " km " + m + " m " + cm + " cm");
    }

    public static void main(String[] args) {
        Distance1 d1 = new Distance1();
        Distance1 d2 = new Distance1();
        Distance1 result = new Distance1();

        d1.input(2, 500, 50);
        d2.input(1, 800, 70);

        result.add(d1, d2);
        result.display();
    }
}
```
<img width="187" height="21" alt="Screenshot 2026-03-12 223136" src="https://github.com/user-attachments/assets/46a06249-74b6-4b58-902c-7b7cfd1c9897" />
]
#assci-4

## assci-5
[
```
class Distance2 {
    int m, cm;

    void input(int m, int cm) {
        this.m = m;
        this.cm = cm;
    }

    void add(Distance2 d1, Distance2 d2) {
        cm = d1.cm + d2.cm;
        m = d1.m + d2.m + cm / 100;
        cm = cm % 100;
    }

    void display() {
        System.out.println(m + " meter " + cm + " cm");
    }

    public static void main(String args[]) {

        Distance2 d1 = new Distance2();
        Distance2 d2 = new Distance2();
        Distance2 result = new Distance2();

        d1.input(5, 80);
        d2.input(3, 40);

        result.add(d1, d2);
        result.display();
    }
}
```
<img width="164" height="26" alt="image" src="https://github.com/user-attachments/assets/8e302576-fba7-45d5-a372-e72b2facd3fa" />
]
#assci-5

## assci-6
[
```
class Factorial {
    void fact(int n) {
        int f = 1;

        for(int i = 1; i <= n; i++) {
            f = f * i;
        }

        System.out.println("Factorial = " + f);
    }

    public static void main(String args[]) {
        Factorial obj = new Factorial();
        obj.fact(5);
    }
}
```
<img width="179" height="23" alt="Screenshot 2026-03-12 223710" src="https://github.com/user-attachments/assets/8ed3b4d5-4fdb-466c-8a8f-46a77e3f6d63" />
]
#assci-6
