# Stop Watch in x86 Assembly Language

## Description
![description1](../master/images/p1.png)

![description2](../master/images/p2.png)

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
4- Now to run the code, run DOSBOX 0.74 and type
```
nasm timer.asm -o timer.com  
```
```
afd timer.com
```
