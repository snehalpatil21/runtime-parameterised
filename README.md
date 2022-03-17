# runtime-parameterised
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace constructor89
{
    class Program
    {
        //c# program to illustrate calling
        //a default constructor
        int num;
        string name;
        //this would be invoked while the object of class created.
        Program(int a,string b)
        {
            num = a;
            name = b;
            Console.WriteLine("hello");
        }
        //main method
        static void Main(string[] args)
        {
            int a;
            string b;
            Console.WriteLine("enter number:");
            a = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("enter name:");
            b = Convert.ToString(Console.ReadLine());
            //this would invoke default  //constructor.
            Program p = new Program(a,b);
             //default constructor provides //the default values to the //int and object.
            Console.WriteLine(p.name);
            Console.WriteLine(p.num);
            Console.ReadLine();
        }
    }
}
