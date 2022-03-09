# CMPE140Project1

First of all, Our inputs R1 is dividend, R2 is divisor. We gave R5 is always 1, others are 0. First step, we copied R1 and R2 values to M1 and M2.
Then, we are going to compare R1 and R2, if R1<R2 then R6 will be 1, otherwise 0. If R6 is 1, we are moving to 8th line. This subalgoritm named "IsSmaller".
If R6 is 0, now we will check R1 and R2 is equal or not. If they are equal, R6 will be 1, and we are moving to 10th line. This subalgorithm named "IsEqual".
If R6 is again 0, there is one chance which is R1>R2. Now we are in the 7th line. This subalgorithm named "IsBıgger". If we get R3:0 in this subalgorithm, we will move to 8th line.
Then, we will do the steps in IsSmaller. If this subalgorithm gives R3:1 output, we will move to 11th line. In 11th line we are changing the registers in correct place because our remainder is in R1, our quotient is in R4 right now.
If the IsSmaller gives R3:0 output, we will go to 10th step, This subalgorithm called "IsEqual". We will do steps in this subalgorithm. 
Now we are in 11th line, and we are changing the registers in correct place because our remainder is in R1, our quotient is in R4 right now.
