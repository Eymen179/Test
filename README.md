# Test

using System;

class Program
{
    static void Main()
    {
        for (int i = 500; i <= 599; i++)
        {
            if (IsPrime(i))
            {
                Console.WriteLine(i);
            }
        }
    }
    
    static bool IsPrime(int number)
    {
        if (number < 2)
            return false;
        for (int i = 2; i <= Math.Sqrt(number); i++)
        {
            if (number % i == 0)
                return false;
        }

        return true;
    }
}
