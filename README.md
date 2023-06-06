# Inheritance
# Aim:
To write a C# program to print some messages using hierarchical inheritance.

# Algorithm:
Step 1:
Create a base class.

Step 2:
Create two child class.

Step 3:
Create a constructor in the base class and print a message.

Step 4:
Create constructor in child classes to print the message.

## Program:
Developed by VISMAYA.S
Register no: 212221230125
```
using System;

namespace exp8
{
    public class tyre
    {
        public tyre()
        {
            Console.WriteLine("Tyre - Vehicle");
        }
        public virtual void display()
        {
            Console.Write("Tyre is attached to ");
        }
    }

    public class car : tyre
    {
        public car()
        {
            Console.WriteLine("Car Constructor");
        }
        public override void display()
        {
            base.display();
            Console.WriteLine("Car");
        }
    }

    public class scooter : tyre
    {
        public scooter()
        {
            Console.WriteLine("Scooter Constructor");
        }
        public override void display()
        {
            base.display();
            Console.WriteLine("Scooter");
        }
    }
    public class main
    {
        public static void Main(string[] args)
        {
            car newcar = new car();
            newcar.display();

            Console.WriteLine();

            scooter newscooter = new scooter();
            newscooter.display();
        }
    }
}
```

## Output:
![image](https://github.com/VismayaNair/Inheritance/assets/93427210/150d5622-f32b-45ec-8a48-f4520a0f3546)



## Result
Thus, C# program to print some messages using hierarchical inheritance is implemented successfully.
