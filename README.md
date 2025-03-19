using System;

class Calculator
{
    static void Main(string[] args)
    {
        double num1, num2, result;
        string operation;

        Console.WriteLine("Simple Calculator");

        Console.Write("Enter the first number: ");
        num1 = Convert.ToDouble(Console.ReadLine());

        Console.Write("Enter the second number: ");
        num2 = Convert.ToDouble(Console.ReadLine());

        
        Console.Write("Enter the operation (+, -, *, /): ");
        operation = Console.ReadLine();

       
        switch (operation)
        {
            case "+":
                result = num1 + num2;
                Console.WriteLine($"The result of {num1} + {num2} is: {result}");
                break;
            case "-":
                result = num1 - num2;
                Console.WriteLine($"The result of {num1} - {num2} is: {result}");
                break;
            case "*":
                result = num1 * num2;
                Console.WriteLine($"The result of {num1} * {num2} is: {result}");
                break;
            case "/":
                if (num2 != 0)
                {
                    result = num1 / num2;
                    Console.WriteLine($"The result of {num1} / {num2} is: {result}");
                }
                else
                {
                    Console.WriteLine("Error! Division by zero is not allowed.");
                }
                break;
            default:
                Console.WriteLine("Invalid operation! Please use +, -, *, or /.");
                break;
        }
    }
}
# calculator-program-in-c-
