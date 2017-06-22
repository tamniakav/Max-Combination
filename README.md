using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Max_Combination
{
    class Program
    {
        static void Main(string[] args)
        {
            int beginning = int.Parse(Console.ReadLine());
            int end = int.Parse(Console.ReadLine());
            int stop = int.Parse(Console.ReadLine());

            int counter = 0;

            for (int i = beginning; i <= end; i++)
            {
                for (int j = beginning; j <= end; j++)
                {
                    Console.Write($"<{i}-{j}>");
                    counter++;

                    if (counter == stop)
                    {
                        break;
                    }
                }
                if (counter == stop)
                {
                    break;
                }
            }
            Console.WriteLine();
        }
    }
}
