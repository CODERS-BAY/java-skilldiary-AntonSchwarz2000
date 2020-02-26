## java day 4


I finished the maximum example.

    package com.codersbay;

    import java.util.Scanner;

    public class Main {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int[] numbers = new int[0];

        while (!scanner.hasNext("q") && !scanner.hasNext("Q")) {
            int newNumber = scanner.nextInt();
            int[] biggerArray = new int[numbers.length + 1];

            for (int i = 0; i < numbers.length; i++) {
                biggerArray[i] = numbers[i];
            }
            biggerArray[numbers.length] = newNumber;
            numbers = biggerArray;
        }

        int biggestNumber = 0;
        for (int i = 0; i < numbers.length; i++) {
            if (biggestNumber < numbers[i]) {
                biggestNumber = numbers[i];
            }
        }

        System.out.println("you entered q or Q");
        System.out.println("maximum is  " + biggestNumber);

        }   
        }
    }        


I finished the insertion sort.


    package com.codersbay;

    import java.util.Arrays;

    public class Main {

    public static void main(String[] args) {
        int[] unsorted = {12, 234, -2, 24, -234};
        int[] sorted = insertionSort (unsorted) ;
        for (int i = 0; i < sorted.length; i++) {
            System.out.println(sorted[i] + ",  ");
        }
    }
    public static int[] insertionSort (int[] sort) {
        int temp;
        for (int i = 1; i < sort.length; i++) {
            temp = sort[i];
            int j = i;
            while (j > 0 && sort[j - 1] > temp) {
                sort[j] = sort[j - 1];
                j--;
            } sort[j] = temp;
        } return sort;
    }

    }   


I started working with the bubble sort.