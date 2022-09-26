using System;
using System.Security.Cryptography;
Console.WriteLine("Введите номер действия: ");
Console.WriteLine("1. Сложить");
Console.WriteLine("2. Вычесть");
Console.WriteLine("3. Умножить");
Console.WriteLine("4. Разделить");
Console.WriteLine("5. Возвести в степень N первое число");
Console.WriteLine("6. Найти квадратный корень из числа");
Console.WriteLine("7. Найти 1 процент от числа");
Console.WriteLine("8. Найти факториал из числа");
Console.WriteLine("9. Выйти");
Console.WriteLine("Введите 1 число");
double NumOdin = Convert.ToDouble(Console.ReadLine());
Console.WriteLine("введите 2 число");
double NumDva = Convert.ToDouble(Console.ReadLine());
Console.WriteLine("введите номер операции");
double Num = Convert.ToDouble(Console.ReadLine());

while (Num <= 8)
  
{
    switch (Num)
    {
        case 1:
            Console.Write("ответ: ");
            Console.WriteLine(NumOdin + NumDva);
            break;
        case 2:
            Console.Write("ответ: ");
            Console.WriteLine(NumOdin - NumDva);
            break;
        case 3:
            Console.Write("ответ: ");
            Console.WriteLine(NumOdin * NumDva);
            break;
        case 4:
            Console.Write("ответ: ");
            Console.WriteLine(NumOdin / NumDva);
            break;
        case 5:
            Console.Write("ответ: ");
            Console.WriteLine(Math.Pow(NumOdin, NumDva));
            break;
        case 6:
            Console.Write("ответ: ");
            Console.WriteLine(Math.Sqrt(NumOdin));
            break;
        case 7:
            Console.Write("ответ: ");
            Console.WriteLine(NumOdin * 0.01);
            break;
        case 8:
            Console.Write("ответ: ");

            int f = 1;
            int i;
            for (i = 2; i <= NumDva; i++)
            {
                f = f * i;
            }
            Console.WriteLine(f);
            break;
    }
    Console.WriteLine("введите операцию");
    Num = Convert.ToDouble(Console.ReadLine());
}
