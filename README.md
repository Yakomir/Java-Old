package ru.geekbrains.java;

public class Lesson_2

***** №1 *****
    {
        public static void invertArrayZeroToOneOneToZero
    {
        System.out.println("Задание №1. Задать целочисленный массив, состоящий из элементов 0 и 1. Например: [ 1, 1, 0, 0, 1, 0, 1, 1, 0, 0 ]. С помощью цикла и условия заменить 0 на 1, 1 на 0;")ж
        
        int[] a = {1, 1, 0, 0, 1, 0, 1, 1, 0, 0};
        for (int i = 0; i <= 9; i++)
        {
            if (a[i] == 0)
            {
                a[i]++;
            }
            else
            {
                a[i]--;
            }
            System.out.println(a[i]);
        }

***** №2 *****

    public static void arraySimpleAriphmeticIncrease
    {
            System.out.println("Задание №2. Задать пустой целочисленный массив размером 8. С помощью цикла заполнить его значениями 0 3 6 9 12 15 18 21;");
        
        int[] a = new int[8];
        for (int i = 0, j = 0; i <= a.length; i++, j+= 3)
        {
            a[i] = j;
            System.out.println(j);
        }

    }
    
    ***** №3 *****
    
      public static void detectionAndDoubleDigitslessThenSix
    {
            System.out.println("Задание №3. Задать массив [ 1, 5, 3, 2, 11, 4, 5, 2, 4, 8, 9, 1 ] пройти по нему циклом, и числа меньшие 6 умножить на 2");
        
        int[] a = {1, 5, 3, 2, 11, 4, 5, 2, 4, 8, 9, 1 };
        for (int i = 0; i <= a.length; i++)
        {
            if (a[i] < 6)
            {
                a[i] = a[i] * 2;
            }
            System.out.println(a[i]);
     }       
 }   
 
 ****** №4 *****
 
 public static void main (String[] args)
    {
        System.out.println("Задание №4. Создать квадратный двумерный целочисленный массив (количество строк и столбцов одинаковое), и с помощью цикла(-ов) заполнить его диагональные элементы единицами;");
        System.out.println();
        int[][] a = new int [9][9];

        for (int i = 0; i < a.length; i++)
        {
            for (int j = 0; j < a[i].length; j++)
            {
                if ((i==j)||(i==a.length - 1 -j))
                    a[i][j] = 1;
                System.out.print(a[i][j]);
            }
            System.out.println();
        }

    }
    
    ****** №5 *****
    
    public static void main (String[] args)
    {
        System.out.println("Задание №5. Задать одномерный массив и найти в нем минимальный и максимальный элементы (без помощи интернета)");
        System.out.println();
        int[] array = {19, 23, 6, 17, 9, 37, 45, 2, 11};
        int minValue = array[0];
        int maxValue = array[0];

        int minIndex = 0;
        int maxIndex = 0;

        for (int i = 1; i<array.length; i++)
        {
            if (array[i] < minValue)
            {
                minValue = array[i];
                minIndex = i;
            }
            else if (array[i] > maxValue)
            {
                maxValue = array[i];
                maxIndex = i;
            }
        }
        System.out.println("Минимальное значение в массиве: " + minValue);
        System.out.println("Индекс минимального значения: " + minIndex);
        System.out.println();
        System.out.println("Максимальное значение в массиве: " + maxValue);
        System.out.println("Индекс максимального значения: " + maxIndex);
    }
    
    ***** №6 *****
    
    
