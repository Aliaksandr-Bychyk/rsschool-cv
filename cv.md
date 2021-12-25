
# Aliaksandr Bychyk

## Contacts

__Phone__: +375292288506

__Email__: sanya55bychyk@gmail.com

__GitHub__: [AlexanderBychyk](https://github.com/AlexanderBychyk)

__Discord__: AmazingSanya#7830

__Telegram__: [alexander_bychyk](https://t.me/alexander_bychyk)

***

## Basic known skills

* HTML
* CSS/SASS
* JavaScript
* Pascal
* C#
* React
* GitHub
* Visual Studio Code
* NPM

***

## C# code example

```C#

using System;

namespace lab9{
  class Program{
    static void Main(string[] args){
      Console.Write("Дан прямоугольный массив A[1..N, 1..M].\nВведитче целое число N: ");
      int numbN = int.Parse(Console.ReadLine());
      Console.Write("Введите число M: ");
      int numbM = int.Parse(Console.ReadLine());
      Console.WriteLine("Введите диапозон [a..b]: ");
      Console.Write("Введите a: ");
      int randDown = int.Parse(Console.ReadLine());
      Console.Write("Введите b: ");
      int randUp = int.Parse(Console.ReadLine());

      int[,] arrayA = new int[numbN, numbM];
      int[] arrayB = new int[numbN];

      Console.WriteLine("A[1..{0}, 1..{1}]: ", numbN, numbM);
      Random randomGen = new Random();
      for (int i = 0; i<=numbN-1; i++){
        for (int j = 0; j<=numbM-1; j++){
          arrayA[i,j] = randomGen.Next(randDown,randUp);
          Console.Write("[{0}]", arrayA[i,j]);
        }
        for (int j = 0; j<=numbM-1; j++){
          for (int k = j+1; k<=numbM-1; k++){
            if (arrayA[i,j] == arrayA[i,k]) {
              Console.Write(":+:");
              arrayB[i]=i+1;
            }
          }
        }
        Console.WriteLine();
      }

      Console.Write("\n---\n");

      for (int i = 0; i<=numbN-1; i++){
        if (arrayB[i] != 0){
          Console.Write("[{0}]", arrayB[i]);
        }
      }

      Console.ReadKey();
    }
  }
}

```

***

## Experience

I don't have any experience at working on a company. I works only on my own projects.

***

## Aducation

__University__: Brest State A.S. Pushkin University
