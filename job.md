// Задача 34. Задайте массив заполненный случайными  положительными трехзначными числами.
//Напишите программу, которая покажет колличество чётных чисел в массиве.
//[345, 897, 568, 234] -> 2

void InputArray (int [] array)
{
    for (int i =1; i< array.Length; i++)
        array[i] = new Random().Next(100,1000);
}
int ReleaseArray (int [] array)
{
    int count = 0;
    for (int i =1; i< array.Length; i++)
        if (array[i]%2=0) Count+=1;
    return 0;

}
Console.WrineLine("Введи колличество элементов массива n =:");
int n = ConvertToInt32(Console.ReadLine());
int [] array = new int [n];

InputArray (array);
Console.WrineLine($"[{string.Join(", " array)}]");
Console.WrineLine(ReleaseArray (array));