# newc-using System;
using System.Collections;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    class Program
    {

        public void addanimal(ArrayList cnames, ArrayList ccolor, ArrayList gnames, ArrayList gcolor)
        {
            int option;
            string name, color;
            //bool a, b;
            Console.WriteLine("1: Cow");
            Console.WriteLine("2: Goat");
            option = Convert.ToInt32(Console.ReadLine());
            switch (option)
            {
                case 1:
                    AddCow(cnames, ccolor);
                    break;
                case 2:
                    AddGoat(gnames, gcolor);
                    break;
                default:
                    Console.WriteLine("Wrong Option");
                    break;


            }

        }

        private void AddGoat(ArrayList gnames, ArrayList gcolor)
        {
            throw new NotImplementedException();
        }

        private void AddCow(ArrayList cnames, ArrayList ccolor)
        {
            throw new NotImplementedException();
        }

        public void AddCow(ArrayList cnames, ArrayList ccolor, ArrayList gnames)
        {
            string name, color;
            bool a, b;
            Console.WriteLine("Enter cow name");
            name = Console.ReadLine
                ();
            a = cnames.Contains(name);
            b = gnames.Contains(name);
            if (a || b)

            {
                Console.WriteLine("Animal is already present");

            }
            else
            {
                cnames.Add(name);
                Console.WriteLine("Enter the color of cow");
                color = Console.ReadLine();
                object Color = null;
                ccolor.Add(Color);
            }
        }

        private class ConsoleApp1
        {
           
            static void Main(string[] args)
            {

                int farmland;
                Program farm = new Program();
                ArrayList cnames = new ArrayList(100);
                ArrayList ccolor = new ArrayList(100);
                ArrayList gnames = new ArrayList(100);
                ArrayList gcolor
                    = new ArrayList(100);
                do
                {

                    Console.WriteLine("Welcome to farmland");
                    Console.WriteLine("1:Add an animal");
                    Console.WriteLine("2:Show all the animals");
                    Console.WriteLine("3:Sort animal by name");
                    Console.WriteLine("4:Exit from the farmland");
                    farmland = Convert.ToInt32(Console.ReadLine());

                    if (farmland == 4)
                    {
                        Console.WriteLine("Thankyou for visiting the farmland");
                        break;
                    }

                    else
                    {
                        switch (farmland)
                        {
                            case 1:
                                farm.addanimal(cnames, ccolor, gnames, gcolor);
                                break;
                            case 2:
                                farm.showanimal(cnames, gnames);
                                break;
                            case 3:
                                farm.sortanimal(cnames, gnames);
                                break;
                            default:
                                Console.WriteLine("Enter the correct option from \n1 \n2 \n3 \n4");
                                Console.ReadLine();
                                break;
                        }
                    }
                }
                while (true);




            }

            public override bool Equals(object obj)
            {
                return base.Equals(obj);
            }

            public override int GetHashCode()
            {
                return base.GetHashCode();
            }

            public override string ToString()
            {
                return base.ToString();
            }
        }

        private void sortanimal(ArrayList cnames, ArrayList gnames)
        {
            throw new NotImplementedException();
        }

        private void showanimal(ArrayList cnames, ArrayList gnames)
        {
            throw new NotImplementedException();
        }
    }
}
