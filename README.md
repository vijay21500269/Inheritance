# Inheritance

## Aim:
To write a C# program to print some messages using hierarchical inheritance


## Algorithm:
Step 1:
Create a base class Tyre.

Step 2:
Create two child class.

Step 3:
Create a constructor in the base class and print a message.

Step 4:
create a function in child class to print a message.

Step 5:
Run the program.

## Program:
~~~
using System;
namespace vehicles
{
    public class tyre
    {
        public tyre()
        {
            Console.WriteLine("base class tyre");
        }
        public virtual void Display()
        {
            Console.WriteLine("tyre");
        }

    }
    public class scooter : tyre
    {
        public scooter()
        {
            Console.WriteLine("child class Scooter");
        }
        public override void Display()
        {
            base.Display();
            Console.WriteLine("scooter");
        }
    }
    public class car : tyre
    {
        public car()
        {
            Console.WriteLine("child class car");
        }
        public override void Display()
        {
            base.Display();
            Console.WriteLine("car");
        }
    }
    public class hello
    {
        static void Main(string[] args)
        {
            car ar = new car();
            scooter sc = new scooter();
            ar.Display();
            sc.Display();

        }
    }


}
~~~

## Output:
![img](https://github.com/vijay21500269/Inheritance/blob/main/Exp8.png)

## Result
C# program to print some messages using hierarchical inheritance is implemented successfully.


