# Single-Inheritance-in-java
import java.util.Scanner;
class A 
{
    int age;
    int id;

    void getdata()
    {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter your age");// Input data
        age = sc.nextInt();
        System.out.println("Enter our id");
        id = sc.nextInt();
    }
}
class B extends A{
    void showdata() // show data
    {
        System.out.println("Person age is: "+age);
        System.out.println("Person id is: "+id);
    }
}
class SI 
{
    public static void main(String[] args)
    {
        B b1 = new B();
        b1.getdata();
        b1.showdata();
    }
}
