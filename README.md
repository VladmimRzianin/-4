//14
        Console.Write("целое число N > 0 ");
        int N = int.Parse(Console.ReadLine());

        if (N <= 0)
        {
            Console.WriteLine("число должно быть больше 0");
            return;
        }

        int square = 0;
        for (int i = 1; i <= 2 * N - 1; i += 2)
        {
            square += i;
        }

        Console.WriteLine($"Квадрат числа {N} равен {square}");

//21

        int x = int.Parse(Console.ReadLine()); int g = 0;
        int r = 0;
        if (x > 10)
        {
            while (x > 9)
            {
                g = x % 2;
                if (g != 0)
                {
                    r += 1;
                }
                x = x / 10;
            }
            if (r > 0)
            {
                Console.WriteLine("True");
            }
            else
            {
                Console.WriteLine("False");
            }
        }
        else
        {
            g = x % 2; if (g == 0)
            {
                Console.WriteLine("False");
            }
            else
            {
                Console.WriteLine("True");
            }
        }

//18

        Console.Write("количество элементов N ");
        int y = int.Parse(Console.ReadLine());

        Console.WriteLine("элементы набора по одному числу ");
        int[] numbers = new int[y];

        for (int i = 0; i < y; i++)
        {
            numbers[i] = int.Parse(Console.ReadLine());
        }

        Console.WriteLine("результат с уникальными элементами");

        Console.WriteLine(numbers[0]);  

        for (int i = 1; i < y; i++)
        {
            if (numbers[i] != numbers[i - 1])
            {
                Console.WriteLine(numbers[i]);
            }
        }
