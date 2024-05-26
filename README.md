# Longest Increasing Subsequence Finder

This project provides a Java implementation for dynamically finding all longest increasing subsequences within a given array of integers.

## Description

Given an array of integers, the program finds all possible longest subsequences that are in increasing order. For example, if the input array is `[0, 4, 3, 6, 5, 7, 8]`, the output can be:

- `[0, 3, 5, 7, 8]`
- `[0, 4, 5, 7, 8]`
- `[0, 4, 6, 7, 8]`
- And other possible longest increasing subsequences.

## How It Works

The program uses dynamic programming to efficiently compute the longest increasing subsequences. It maintains a list of lists to store the increasing subsequences found at each position in the array. The algorithm iterates through the array and builds these subsequences by comparing each element with previous elements to find increasing patterns.

## Getting Started

### Prerequisites

- Java Development Kit (JDK) installed on your system.
- A Java IDE or text editor to run the code (e.g., IntelliJ IDEA, Eclipse, VSCode).

### Running the Program

1. **Clone the repository or download the `DynamicSubsequence.java` file.**

2. **Compile and run the Java program:**

   ```sh
   javac DynamicSubsequence.java
   java DynamicSubsequence
   ```

3. **The program will output the longest increasing subsequences for the given array:**

   ```sh
   [0, 4, 6, 7, 8]
   [0, 4, 5, 7, 8]
   [0, 3, 5, 7, 8]
   ```

### Customizing the Input

To test the program with different input arrays, modify the `nums` array in the `main` method:

```java
public static void main(String[] args) {
    int[] nums = {your, custom, array, values};
    List<List<Integer>> lis = findLIS(nums);
    for (List<Integer> seq : lis) {
        System.out.println(seq);
    }
}
```

## Example

```java
public static void main(String[] args) {
    int[] nums = {1, 2, 1, 5, 2, 6, 7, 8};
    List<List<Integer>> lis = findLIS(nums);
    for (List<Integer> seq : lis) {
        System.out.println(seq);
    }
}
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Algorithm inspired by common dynamic programming approaches for finding longest increasing subsequences.
- Java documentation and community forums for support.