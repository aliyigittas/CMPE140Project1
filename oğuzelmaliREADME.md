R1: Dividend
R2: Divisor
R3:0
R4:1
M1: 0
M2: 0
1)	Read/Write(r1,m1)  
2)	Read/Write(r2,m2)      
3)	>=(r1,r2,r5)        
4)	sub(r1,r5,r1)             
5)	Add(r3,r5,r3)                        
6)	Ifjump(r5,3)             
7)	Read/Write(r1, m1) 
8)	Read/Write(r3, m2)  
End===> r3: Quotient r1: Remainder
