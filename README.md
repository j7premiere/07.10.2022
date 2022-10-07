### Task 7 kyu

[Task link](https://www.codewars.com/kata/58aed2cafab8faca1d000e20/)

You are provided with an array of positive integers and an additional integer n (n > 1).

Calculate the sum of each value in the array to the nth power. Then subtract the sum of the original array.

### My solution

```Java

public class Kata {
    public static int modifiedSum(int[] array, int power) {
        int sum = 0;
        for (int n : array) {
            sum += Math.pow(n,power) - n;
        }
        return sum;
    }
}

```

### Favourite solution from code-wars

```Java

public class Kata {
    public static int modifiedSum(int[] array, int power) {
        return Arrays.stream(array).map(x -> (int)Math.pow(x, power) - x).sum();
    }
}

```

We have the same solution, so I like it, haha

# Have a nice day!