# Highest Value Palindrome

Palindromes are strings that read the same from the left or right, for example madam or 0110.

You will be given a string representation of a number and a maximum number of changes you can make. Alter the string, one digit at a time, to create the string representation of the largest number possible given the limit to the number of changes. The length of the string may not be altered, so you must consider 's left of all higher digits in your tests. For example 0110 is valid, 0011 is not.

Given a string representing the starting number and a maximum number of changes allowed, create the largest palindromic string of digits possible or the string -1 if it's impossible to create a palindrome under the contstraints.

Function Description

Complete the highestValuePalindrome function in the editor below. It should return a string representing the largest value palindrome achievable, or -1.

highestValuePalindrome has the following parameter(s):

s: a string representation of an integer

n: an integer that represents the length of the integer string

k: an integer that represents the maximum number of changes allowed

Input Format

The first line contains two space-separated integers,  and , the number of digits in the number and the maximum number of changes allowed. 

The second line contains an -digit string of numbers.

Constraints

0 ≤ n ≤ 10^5

0 ≤ k ≤ 10^5

Each character i in the number is an integer where 0 ≤ i ≤ 9

Output Format

Print a single line with the largest number that can be made by changing no more than  digits. If this is not possible, print -1.

Sample Input 0

```
4 1
3943
```

Sample Output 0

```
3993
```

Sample Input 1

```
6 3
092282
```

Sample Output 1

```
992299
```

Sample Input 2

```
4 1
0011
```

Sample Output 2

```
-1
```

Test Cases:
```
        highestValuePalindrome("3943", 4, 1); //3993
        highestValuePalindrome("092282", 6, 3); //992299
        highestValuePalindrome("0011", 4, 1); //-1
        highestValuePalindrome("10011", 5, 1); //11011
        highestValuePalindrome("10011", 5, 3); //91019
        highestValuePalindrome("1111911", 7, 4); //9199919
        highestValuePalindrome("329", 3, 2); //999
        highestValuePalindrome("932239", 6, 2); //992299
        highestValuePalindrome("11119111", 8, 4); //91199119
        highestValuePalindrome("11117111", 8, 3); //91177119
        highestValuePalindrome("11117111", 8, 3); //91177119
        highestValuePalindrome("9711319", 7, 4); //9991999
        highestValuePalindrome("1111111", 7, 4); //9911199
        highestValuePalindrome("128392759430124", 15, 8); //929394959493929
```
