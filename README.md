# FizzBuzz
Solution

using System;


namespace FizzBuzz
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.Write("Please enter the number that you wish to count to: ");            
            int maxNumber = Convert.ToInt16(Console.ReadLine());
            Console.WriteLine();

            for (int i = 1; i < (maxNumber+1); i++)
            {
                
                if (i % 3 == 0 && i % 5 == 0) Console.WriteLine("FizzBuzz");
                else if (i % 3 == 0) Console.WriteLine("Fizz");
                else if (i % 5 == 0) Console.WriteLine("Buzz");
                else Console.WriteLine(i);
            }
            
            Console.WriteLine("Press any key to exit");
            Console.ReadKey();
        }
    }
}
