[program-1 for calculator ](#code1)
[program-2 for HelloWorld ](#code2)
[program-3 for Armstrong ](#code3)
[program-4 for Distance1 ](#code4)
[program-5 for Distance2 ](#code5)
[program-6 for Factorial ](#code6)
[program-7 for Fibonacci ](#code7)
[program-8 for Main ](#code8)
[program-9 for Palindrome ](#code9)
[program-10 for Pattern ](#code10)
[program-11 for ReverseArray ](#code11)
[program-12 for Time1 ](#code12)
[program-13 for Time2 ](#code13)
[program-14 for SingleInheritanceDemo ](#code14)
[program-15 for MultilevelInheritanceDemo ](#code15)
[program-16 for HierarchicalInheritanceDemo ](#code16)
## assci-1

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

## assci-2

```
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```
<img width="138" height="38" alt="image" src="https://github.com/user-attachments/assets/36572a87-731d-4a6e-b18e-9ab856a6f314" />


## assci-3
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

## assci-4
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

## assci-5
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

## assci-6
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

## assci-7
```
class Fibonacci {

    void series(int n) {
        int a = 0, b = 1;

        for(int i = 1; i <= n; i++) {
            System.out.print(a + " ");
            int c = a + b;
            a = b;
            b = c;
        }
    }

    public static void main(String args[]) {
        Fibonacci obj = new Fibonacci();
        obj.series(10);
    }
}
```
<img width="262" height="17" alt="Screenshot 2026-03-12 225430" src="https://github.com/user-attachments/assets/3e00c7ee-2827-4e2f-9fd3-98b93fa2c2c3" />

## assci-8
[
```
class Matrix {
    int a[][] = {
        {1,2,3},
        {4,5,6},
        {7,8,9}
    };

    int b[][] = {
        {1,1,1},
        {1,1,1},
        {1,1,1}
    };

    int c[][] = new int[3][3];

    void sum() {
        System.out.println("Sum of matrices:");
        for(int i=0;i<3;i++){
            for(int j=0;j<3;j++){
                c[i][j] = a[i][j] + b[i][j];
                System.out.print(c[i][j] + " ");
            }
            System.out.println();
        }
    }

    void multiply() {
        System.out.println("Multiplication of matrices:");
        for(int i=0;i<3;i++){
            for(int j=0;j<3;j++){
                c[i][j] = 0;
                for(int k=0;k<3;k++)
                    c[i][j] += a[i][k] * b[k][j];
                System.out.print(c[i][j] + " ");
            }
            System.out.println();
        }
    }

    void transpose() {
        System.out.println("Transpose:");
        for(int i=0;i<3;i++){
            for(int j=0;j<3;j++)
                System.out.print(a[j][i] + " ");
            System.out.println();
        }
    }

    void rowSum() {
        for(int i=0;i<3;i++){
            int sum=0;
            for(int j=0;j<3;j++)
                sum += a[i][j];
            System.out.println("Row " + i + " sum = " + sum);
        }
    }

    void columnSum() {
        for(int j=0;j<3;j++){
            int sum=0;
            for(int i=0;i<3;i++)
                sum += a[i][j];
            System.out.println("Column " + j + " sum = " + sum);
        }
    }

    void diagonalSum() {
        int sum=0;
        for(int i=0;i<3;i++)
            sum += a[i][i];
        System.out.println("Diagonal sum = " + sum);
    }
}

public class Main {
    public static void main(String args[]) {

        Matrix obj = new Matrix();   // object creation

        obj.sum();
        obj.multiply();
        obj.transpose();
        obj.rowSum();
        obj.columnSum();
        obj.diagonalSum();
    }
}
```
<img width="314" height="494" alt="image" src="https://github.com/user-attachments/assets/d92a6697-bf11-44d2-b69b-2eb284999eac" />

## assci-9
```
class Palindrome {

    void check(int n) {
        int rev = 0, r, temp = n;

        while(n > 0) {
            r = n % 10;
            rev = rev * 10 + r;
            n = n / 10;
        }

        if(temp == rev)
            System.out.println("Palindrome");
        else
            System.out.println("Not Palindrome");
    }

    public static void main(String args[]) {
        Palindrome obj = new Palindrome();
        obj.check(121);
    }
}
```
<img width="126" height="27" alt="Screenshot 2026-03-12 230028" src="https://github.com/user-attachments/assets/cf2f438c-df8b-434c-9251-eb6c7c2a4124" />

## asssci-10
```
class Pattern {

    void printPattern() {

        for(int i=1;i<=5;i++) {
            for(int j=1;j<=i;j++) {
                System.out.print("* ");
            }
            System.out.println();
        }
    }

    public static void main(String args[]) {
        Pattern obj = new Pattern();
        obj.printPattern();
    }
}
```
<img width="120" height="126" alt="Screenshot 2026-03-12 230649" src="https://github.com/user-attachments/assets/c26865c0-486f-42cc-833e-d16f52423f8a" />

## assci-11
```
class ReverseArray {
    void reverse(int arr[]) {
        for (int i = arr.length - 1; i >= 0; i--)
            System.out.print(arr[i] + " ");
    }

    public static void main(String[] args) {
        ReverseArray obj = new ReverseArray();
        int a[] = {10, 20, 30, 40, 50};
        obj.reverse(a);
    }
}
```
<img width="166" height="24" alt="Screenshot 2026-03-12 231132" src="https://github.com/user-attachments/assets/3848e00c-3ab4-4a1c-86f9-8e4faf9b9032" />

##assci-12
```
class Time1 {
    int hr, min, sec;

    void input(int hr, int min, int sec) {
        this.hr = hr;
        this.min = min;
        this.sec = sec;
    }

    void add(Time1 t1, Time1 t2) {
        sec = t1.sec + t2.sec;
        min = t1.min + t2.min + sec / 60;
        sec = sec % 60;
        hr = t1.hr + t2.hr + min / 60;
        min = min % 60;
    }

    void display() {
        System.out.println(hr + " hr " + min + " min " + sec + " sec");
    }

    public static void main(String[] args) {
        Time1 t1 = new Time1();
        Time1 t2 = new Time1();
        Time1 result = new Time1();

        t1.input(2, 45, 50);
        t2.input(1, 30, 30);

        result.add(t1, t2);
        result.display();
    }
}
```
<img width="220" height="21" alt="Screenshot 2026-03-12 231640" src="https://github.com/user-attachments/assets/04ed1b1f-9e34-4fc4-b07a-75cf8db89e32" />

## assci-13
```
class Time2 {
    int hr, min;

    void input(int hr, int min) {
        this.hr = hr;
        this.min = min;
    }

    void add(Time2 t1, Time2 t2) {
        min = t1.min + t2.min;
        hr = t1.hr + t2.hr + min / 60;
        min = min % 60;
    }

    void display() {
        System.out.println(hr + " hour " + min + " minutes");
    }

    public static void main(String args[]) {

        Time2 t1 = new Time2();
        Time2 t2 = new Time2();
        Time2 result = new Time2();

        t1.input(2, 45);
        t2.input(3, 30);

        result.add(t1, t2);
        result.display();
    }
}
```
<img width="199" height="21" alt="Screenshot 2026-03-12 232235" src="https://github.com/user-attachments/assets/a5465b3c-a719-4518-a0c2-ea3b0eb0cec1" />

## assci-14
```
class Animal1 {
    void eat() {
        System.out.println("Animal is eating");
    }
}

class Dog1 extends Animal1 {
    void bark() {
        System.out.println("Dog is barking");
    }
}

public class SingleInheritanceDemo {
    public static void main(String[] args) {
        Dog1 obj = new Dog1();
        obj.eat();
        obj.bark();
    }
}
```
<img width="199" height="44" alt="Screenshot 2026-03-12 233147" src="https://github.com/user-attachments/assets/d0b9156c-94db-4b51-952a-76904d177d93" />

## assci-15
```
class Animal2 {
    void eat() {
        System.out.println("Animal eats food");
    }
}

class Dog2 extends Animal2 {
    void bark() {
        System.out.println("Dog barks");
    }
}

class Puppy2 extends Dog2 {
    void weep() {
        System.out.println("Puppy weeps");
    }
}

public class MultilevelInheritanceDemo {
    public static void main(String[] args) {
        Puppy2 obj = new Puppy2();
        obj.eat();
        obj.bark();
        obj.weep();
    }
}
```
<img width="193" height="83" alt="Screenshot 2026-03-12 233611" src="https://github.com/user-attachments/assets/5421b7e0-4c73-4ed6-bb50-ab04e50ab0ca" />

## assci-16
```
class Animal3 {
    void eat() {
        System.out.println("Animal eats");
    }
}

class Dog3 extends Animal3 {
    void bark() {
        System.out.println("Dog barks");
    }
}

class Cat3 extends Animal3 {
    void meow() {
        System.out.println("Cat meows");
    }
}

public class HierarchicalInheritanceDemo {
    public static void main(String[] args) {
        Dog3 d = new Dog3();
        Cat3 c = new Cat3();

        d.eat();
        d.bark();

        c.eat();
        c.meow();
    }
}
```
<img width="136" height="105" alt="Screenshot 2026-03-12 233911" src="https://github.com/user-attachments/assets/8237048e-e645-4f68-bd53-e76c6e939231" />
