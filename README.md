# Stop Watch in x86 Assembly Language

# Bit Manipulation and Subroutines -8086 Assembly

I solved all these questions and shared the solutions here so that you can have a strong grip on these concepts with ready to run interesting solved problems.

## Reference Book

*The questions are taken from the book [Assembly Language Programming by Belal Hashmi and Junaid Haroon](https://onlinebookpoint.blogspot.com/2016/10/assembly-language-programming-delivered.html)*

Its an excellent book for understanding the language and concepts of 8086 Assembly. It starts from the very basics and then takes you to advanced concepts in an efficient manner. Highly Recommended!

## How to Run
1- Download this code and move the 'assembly_code' folder to C: directory.

2- Install DOSBOX from this link: [Download DOSBOX Emulator](https://www.dosbox.com/download.php?main=1)

3- After complete installation, go to DOSBOX installation directory and run "DOSBox 0.74 Options.bat". This will save you from the pain       of searching the configuration file yourself and will open that file for you.
Copy these lines at the end of that file:
```
mount c: c:\assembly_code 
```  
```
c:
```
4- Now to run any question (say named 'chp4_03.asm'), run DOSBOX 0.74 and type
```
nasm chp4_03.asm -o chp4_03.com  
```
```
afd chp4_03.com
```

## Problems Solved

### Question 1: (Exercise of Chp 4 - Bit Manipulation)
* Q-1. Write a program to swap every pair of bits in the AX register.
* Q-3. Write a program to swap the nibbles in each byte of the AX register.
* Q-4. Calculate the number of one bits in BX and complement an equal number of least significant bits in AX.
* Q-5. Write a program to multiply two 32bit numbers and store the answer in a 64bit location.
* Q-6. Declare a 32byte buffer containing random data. Consider for this problem that the bits in these 32 bytes are numbered from 0 to 255.     Declare another byte that contains the starting bit number. Write a program to copy the byte starting at this starting bit number in the AX register. Be careful that the starting bit number may not be a multiple of 8 and therefore the bits of the desired byte will be split into two bytes.
* Q-7. AX contains a number between 0-15. Write code to complement the corresponding bit in BX. For example if AX contains 6; complement the 6th bit of BX.
* Q-8. AX contains a non-zero number. Count the number of ones in it and store the result back in AX. Repeat the process on the result (AX) until AX contains one. Calculate in BX the number of iterations it took to make AX one.

### Question 2: (Exercise of Chp 5 - Subroutines)
* Q-3. Write a recursive function to calculate the Fibonacci of a number. The number is passed as a parameter via the stack and the calculated Fibonacci number is returned in the AX register. A local variable should be used to store the return value from the first recursive call. Fibonacci function is defined as follows: Fibonacci(0) = 0 Fibonacci(1) = 1 Fibonacci(n) = Fibonacci(n-1) + Fibonacci(n-2)
* Q-4. Write the above Fibonacci function iteratively.
* Q-5. Write a function switch_stack meant to change the current stack and will be called as below. The function should destroy no registers. push word [new_stack_segment] push word [new_stack_offset] call switch_stack
* Q-8. Make an array of 0x80 bytes and treat it as one of 0x400 bits. Write a function myalloc that takes one argument, the number of bits. It p, and returns in AX the index of the first bit. Write another function myfree that takes two arguments, index of a bit in the array, and the number of bits. It makes that many consecutive bits zero, whatever their previous values are, starting from the index in the first argument.

