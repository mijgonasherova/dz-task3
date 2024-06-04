// Задача 3: Задайте произвольный массив. Выведете
// его элементы, начиная с конца. Использовать
// рекурсию, не использовать циклы.
// Пример
// [1, 2, 5, 0, 10, 34] => 34 10 0 5 2 1


void PrintArrayReverse(int[] array, int index)
{
    if(index < 0) return;
    Console.Write(array[index] + " ");
    PrintArrayReverse(array, index - 1);
}

int[] arr = [1, 2, 5, 0, 10, 34];

PrintArrayReverse(arr, arr.Length - 1);

