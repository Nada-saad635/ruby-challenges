
# Missing Number Finder

This Python solution is designed to find a missing number in a list of integers. The list contains numbers in a random order, and one number from the sequence is missing. The goal is to identify and return the missing number.

# Problem Statement

Given a list of integers, where the numbers are supposed to be within a certain continuous range (from the minimum value to the maximum value), find the number that is missing from the sequence.

For example, for the input:

nums = [2, 1, 5, 4, 6, 9, 7, 8, 10]




## Running Tests

To run tests, run the following command

```bash
  npm run test
```



## Steps
--Identify the Minimum and Maximum Values:

The algorithm first finds the smallest (min_val) and largest (max_val) values in the input list. This establishes the expected range of numbers.



--Generate the Full Set:

A complete set of numbers, ranging from min_val to max_val (inclusive), is generated. This set represents the sequence of numbers that should be present in the list.


--Calculate the Sums:


The sum of the generated set (sum_full_set) is computed.
The sum of the numbers in the input list (sum_nums) is also calculated.


--Find the Missing Number:


The missing number is simply the difference between the sum of the full set and the sum of the input list. This works because the only difference between the two sums is the missing number.



    