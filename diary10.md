## java day 5

We discussed an example from the java test last week.

I finished the bubble sort.

    package com.codersbay;

    public class Main {
    public static void main(String[] args) {

        int[] unsorted = {2349, 45, 3, -67, 67, -7};
        int[] sorted = bubbleSort(unsorted);

        for (int i = 0; i < sorted.length; i++) {
            System.out.println(sorted[i] + ",  ");
        }
    }

    public static int[] bubbleSort(int[] sort) {
        int temp;
        for (int i = 1; i < sort.length; i++) {
            for (int j = 0; j < sort.length - i; j++) {
                if (sort[j] > sort[j + 1]) {
                    temp = sort[j];
                    sort[j] = sort[j + 1];
                    sort[j + 1] = temp;
                }
            }
        }
        return sort;
    }
    }


I started the Caesar Chiffre.

We discussed divide and conquer.

Ben and I made a plan for the fibonacci example.