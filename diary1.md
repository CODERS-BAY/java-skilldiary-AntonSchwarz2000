## Java day 1
After almost 2 weeks absence today was my first java day.

I did the FizzBuzz example.

    public class Main {

    public static void main(String[] args) {
        
        for (int i = 1; i <= 100; i++) {
            if (i % 3 == 0 && i % 5 == 0) {
                System.out.println("FizzBuzz");
            } else if (i % 3 == 0) {
                System.out.println("Fizz");
            } else if (i % 5 == 0) {
                System.out.println("Buzz");
            } else {
                System.out.println(i);
            }
        }
    }
}

We discussed Arrays.

We discussed SelectionSort.
        import java.util.Arrays;

        class SelectionSort {
        public static void main(String[] args) {
        int[] numbers = {33, 12, 5, -4, 8, -12, 187};
        System.out.println(Arrays.toString(numbers));
        int startOfUnsorted = 0;

        while(startOfUnsorted < numbers.length) {
            // find local minimum
            int myMinimumIndex = startOfUnsorted;
            int myMinimum = numbers[myMinimumIndex];
            for (int i = startOfUnsorted; i < numbers.length; i++) {
                if (numbers[i] < myMinimum) {
                    myMinimum = numbers[i];
                    myMinimumIndex = i;
                }
            }

            // switch myMinumIndex with startOfUnsorted
            int oldFirst = numbers[startOfUnsorted];
            int newFirst = numbers[myMinimumIndex];
            numbers[myMinimumIndex] = oldFirst;
            numbers[startOfUnsorted] = newFirst;
            System.out.println(Arrays.toString(numbers));

            startOfUnsorted++;
        }
    }
}

We discussed Insertion Sort.

We discussed Merge Sort.

We discussed Quick Sort.