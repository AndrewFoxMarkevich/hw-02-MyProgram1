# hw-02-MyProgram1

using System;
public static class ConversionProgram
{
    static void Main()
    {
        while (true)
        {
            Console.Clear();

            Console.WriteLine("Select data type:byte, sbyte, short, ushort, int, uint, long, ulong");
            string action = Console.ReadLine();

            switch (action)
            {
                case "byte":

                    Console.WriteLine("Input a number");
                    string input = Console.ReadLine();

                    try
                    {
                        byte result = byte.Parse(input);
                        Console.WriteLine(result);
                    }
                    catch (OverflowException)
                    {
                        Console.WriteLine($"Unable to parse '{input}' " +
                            $"becouse  {input} is more {byte.MaxValue} or less {byte.MinValue} ");

                    }
                    break;

                case "sbyte":

                    Console.WriteLine("Input a number");
                    string input1 = Console.ReadLine();

                    try
                    {
                        sbyte result1 = sbyte.Parse(input1);
                        Console.WriteLine(result1);
                    }
                    catch (OverflowException)
                    {
                        Console.WriteLine($"Unable to parse '{input1}' " +
                             $"becouse  {input1} is more then the {sbyte.MaxValue} " +
                             $"or less then the {sbyte.MinValue}");
                    }
                    break;

                case "short":

                    Console.WriteLine("Input a number");
                    string input2 = Console.ReadLine();

                    try
                    {
                        short result2 = short.Parse(input2);
                        Console.WriteLine(result2);
                    }
                    catch (OverflowException)

                    {
                        Console.WriteLine($"Unable to parse '{input2}' " +
                            $"becouse intering number {input2} is more {short.MaxValue} " +
                            $"or less {short.MinValue} ");
                    }
                    break;

                case "ushort":

                    Console.WriteLine("Input a number");
                    string input3 = Console.ReadLine();

                    try
                    {
                        ushort result3 = ushort.Parse(input3);
                        Console.WriteLine(result3);
                    }
                    catch (OverflowException)
                    {
                        Console.WriteLine($"Unable to parse '{input3}' " +
                             $"becouse  {input3} is more then the {ushort.MaxValue} " +
                             $"or less then the {ushort.MinValue}");
                    }

                    break;
            }

            Console.ReadLine();

        }
    }
}
            

   
