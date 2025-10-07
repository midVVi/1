/*Random r = new Random();
int sum = 0;
int[,] arr = new int[3, 3];
for (int i = 0; i < arr.GetLength(0); i++)
{
    for (int g = 0; g < arr.GetLength(1); g++)
    {
        arr[i, g] = r.Next(1, 10);
    }
}
for (int i = 0; i < arr.GetLength(0); i++)
{
    sum = 0;
    for (int g = 0; g < arr.GetLength(1); g++)
    {
        Console.Write(arr[i, g] + " ");
        sum += arr[i, g];
    }
    Console.Write(" | " + sum + " ");
    Console.WriteLine();
}*/

Random r = new Random();
int sum = 0;
int[,] arr = new int[5, 5];
for (int i = 0; i < arr.GetLength(0); i++)
{
    for (int g = 0; g < arr.GetLength(1); g++)
    {
        arr[i, g] = r.Next(1, 10);
    }
}

for (int i = 0; i < arr.GetLength(0); i++)
{
    for (int g = 0; g < arr.GetLength(1); g++)
    {
        Console.Write(arr[i, g] + " ");
    }
    Console.WriteLine();
}

for (int i = 0, g = 0; i < arr.GetLength(0) && g < arr.GetLength(1); i++, g++)
{ 
    sum += arr[i, g];
}

for (int i = 0; i < arr.GetLength(0); i++)
{
    Console.Write("  ");
}
Console.Write(sum);
