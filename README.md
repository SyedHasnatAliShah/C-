using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
 

namespace ConsoleApplication1
{
   public class Program
    {
       static int Fact(int n)
       {

           if (n <= 1)
               return 1;
           else
            return   (n*Fact(n-1));

}
        static void Main(string[] args)
        {
            int i;
            int fact = 1;
            int num;
            int s;
            Console.Write("Press   1:-loop:-        2:-function:-");
            s = int.Parse(Console.ReadLine());
            if (s == 1)
            {
                Console.Write("Enter any number:-");
                num = int.Parse(Console.ReadLine());
                for (i = 1; i <= num; i++)
                {
                    fact = fact * i;
                }
                Console.Write("factorial of:-" + num + "is" + fact);
               
            }
            else if(s==2)
            {
                Console.Write("Enter any number:-");
                num = int.Parse(Console.ReadLine());
                Console.WriteLine(Fact(num));
                Console.ReadKey(true);
            }
        
            Console.ReadKey(true);
        }

    }
}

