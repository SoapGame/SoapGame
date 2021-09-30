using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace DotaBust
{
    class Program
    {
        static void DotaSkriptFirst(ref int yourMmr, ref int purposeMmr, ref int pricesum, ref int  priceFirst, ref int priceSecond, ref int priceThird, ref int priceFourth, ref int priceFifth, ref int priceSixth, ref int priceSeventh, ref int priceEighth, ref int mmrFirst, ref int mmrSecond, ref int mmrThird, ref int mmrFourth, ref int mmrFifth, ref int mmrSixth, ref int mrrSeventh, ref int mmrEighth)
        {


            for (int i = yourMmr; i < purposeMmr; i += 100)
            {
                if (i < mmrFirst)
                {
                    pricesum += priceFirst;
                }
                if (i < mmrSecond && i> mmrFirst)
                {
                    pricesum += priceSecond;
                }
                if (i < mmrThird && i> mmrSecond)
                {
                    pricesum += priceThird;
                }
                if (i < mmrFourth && i> mmrThird)
                {
                    pricesum += priceFourth;
                }
                if (i < mmrFifth && i> mmrFourth)
                {
                    pricesum += priceFifth;
                }
                if (i< mmrSixth&&i> mmrFifth)
                {
                    pricesum += priceSixth;
                }
                if (i< mrrSeventh&&i> mmrSixth)
                {
                    pricesum += priceSeventh;
                }
                if(i< mmrEighth&&i> mrrSeventh)
                {
                    pricesum += priceEighth;
                }
            }
            Console.WriteLine(pricesum);
        }
            
            
        
        static void  Main(string[] args)
        {
          

            int  priceFirst = 200;
            int  priceSecond = 300;
            int priceThird = 400;
            int priceFourth = 450;
            int priceFifth = 600;
            int priceSixth = 800;
            int priceSeventh = 1100;
            int priceEighth = 1500;
            
            int mmrFirst = 4000;
            int mmrSecond = 4500;
            int mmrThird = 5000;
            int mmrFourth = 5500;
            int mmrFifth = 6000;
            int mmrSixth = 6500;
            int mrrSeventh = 7000;
            int mmrEighth = 7500;
            int pricesum = 0;
            int yourMmr = 0;
            int purposeMmr = 0;
            Console.WriteLine("Введите ваш ммр");
            yourMmr = int.Parse(Console.ReadLine());
            Console.WriteLine("Введите желаемый ммр");
            purposeMmr = int.Parse(Console.ReadLine());
            DotaSkriptFirst(ref yourMmr, ref purposeMmr, ref pricesum, ref priceFirst, ref priceSecond, ref priceThird, ref priceFourth, ref priceFifth, ref priceSixth,ref priceSeventh,ref priceEighth,ref mmrFirst,ref mmrSecond,ref mmrThird,ref mmrFourth,ref mmrFifth,ref mmrSixth,ref mrrSeventh,ref mmrEighth) ;
            Console.ReadKey();
            
        }
    }
}
