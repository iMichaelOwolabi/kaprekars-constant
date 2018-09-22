# kaprekars-constant
Kaprekar's Constant implementation in javascript

According too wikipedia https://en.wikipedia.org/wiki/6174_(number) 6174 is known as Kaprekar's constant after the
Indian mathematician D. R. Kaprekar. This number is notable for the following properties :

Take any four-digit number, using at least two different digits. (Leading zeros are allowed.)
  1. Arrange the digits in descending and then in ascending order to get two four-digit numbers, adding leading zeros if necessary.
  2. Subtract the smaller number from the bigger number.
    Go back to step 2 and repeat.

The above process, known as Kaprekar's routine, will usually reach its fixed point, 6174, in at most 8 iterations.
Once 6174 is reached, the process will continue yielding 7641 – 1467 = 6174. For example, choose 3524:

    5432 – 2345 = 3087
    8730 – 0378 = 8352
    8532 – 2358 = 6174
    7641 – 1467 = 6174

The only four-digit numbers for which Kaprekar's routine does not reach 6174 are repdigits such as 1111, which give the 
result 0000 after a single iteration. All other four-digit numbers eventually reach 6174 if leading zeros are used to keep the
number of digits at 4.

This program computes the kaprekar's constant for any valid four digit number as described above and returns the number of steps
it takes for the number to become a kaprekar's constant.
