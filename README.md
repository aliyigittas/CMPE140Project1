# CMPE140Project1

First of all, Our inputs R1 is dividend, R2 is divisor. We gave R5 is always 1, others are 0. First step, we copied R1 and R2 values to M1 and M2.
Then, we are going to compare R1 and R2, if R1<R2 then R6 will be 1, otherwise 0. If R6 is 1, we are moving to 8th line. This subalgoritm named "IsSmaller".
If R6 is 0, now we will check R1 and R2 is equal or not. If they are equal, R6 will be 1, and we are moving to 10th line. This subalgorithm named "IsEqual".
If R6 is again 0, there is one chance which is R1>R2. Now we are in the 7th line. This subalgorithm named "IsBıgger". If we get R3:0 in this subalgorithm, we will move to 8th line.
Then, we will do the steps in IsSmaller. If this subalgorithm gives R3:1 output, we will move to 11th line. In 11th line we are changing the registers in correct place because our remainder is in R1, our quotient is in R4 right now.
If the IsSmaller gives R3:0 output, we will go to 10th step, This subalgorithm called "IsEqual". We will do steps in this subalgorithm. 
Now we are in 11th line, and we are changing the registers in correct place because our remainder is in R1, our quotient is in R4 right now.

IsBıgger

From the memory, we transfer M1 to R1, and from m2 to R2. We compare r1 and r2, if R1 is larger, R3 becomes 1. In the Substract part, we subtract r2 from r1 and write the result to r1. Since R4 is 0 we added 1 (R5). Since R3 is 1, we went back to the if jump step. This time, we check the newly formed R1 with R2, if it is larger again, it writes R3:1 instead of it, if it is smaller or equal, R3:0. We repeat this step until the number is less than the divisor thanks to IfJump. The last comparison results R3:0, but since addition and subtraction operations are performed afterwards, we undo the last operation in next steps. Finally, R1 is registered to M1.


IsSmaller

In this subalgorithm we are checking if R1>R2 or not and gives the result in R3.


IsEqual

In this subalgorithm we are checking if R1=R2 or not and gives the result in R3.




BONUS MULTIPLIFICATION ALGORİTHM

Our inputs are R1 and R2. and we assume that always R3:0, R4:0, R5:1.
In first lines, We are checking if one of the registers are 0, the algorithm will go to the end with 0 result.
Then we will start adding 0 and first number, then we will subtract 1 in the second number, we will repeat the process when we reach 0 in second number.
In the end, our result is stored in R3, we saved this result in M1.
