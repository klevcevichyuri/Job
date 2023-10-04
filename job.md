//    Задача 36. Задайте одномерный массив, заполненный случайными числами.
//Найдите сумму элементов, стоящих на нечетных позициях
//[3, 7, 23, 12] -> 21

void InputArray (int [] array)
{
    for (int i =1; i< array.Length; i++)
        array[i] = new Random().Next(-100,101);
}
int ReleaseArray (int [] array)
{
    int count = 0;
    for (int i =1; i< array.Length; i++)
        count=count + array[i*2+1];
    return count;

}
Console.WriteLine("Введи колличество элементов массива n =:");
int n = ConvertToInt32(Console.ReadLine());
int [] array = new int [n];

InputArray (array);
Console.WriteLine($"[{string.Join(", " array)}]");
Console.WriteLine(ReleaseArray (array));


//    Задача 38. Задайте одномерный массив. Найдите разницу между максимальным
//и минимальным элементами массива
//[3, 7, 22, 2, 78] -> 76

void InputArray (int [] array)
{
    for (int i =1; i< array.Length; i++)
        array[i] = new Random().Next(-100,101);
}
int ReleaseArray (int [] array)
{
    int max = 0;
    int min = 0;
    if ( max > array[i]) array[i] = max;
    else if (min < array[i]) array [i] = min;
    Console.WriteLine( {max-min});

}
Console.WriteLine("Введи колличество элементов массива n =:");
int n = ConvertToInt32(Console.ReadLine());
int [] array = new int [n];

InputArray (array);
Console.WriteLine($"[{string.Join(", " array)}]");
Console.WriteLine(ReleaseArray (array));