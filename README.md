# Digital-Signal-Processing--Convolution
## Aim:
 To perform linear convolution using MAT LAB.
## Software Required:
MAT LAB R2012
## Algorithm:
Step 1: Open mat lab. Write the program.

Step 2: Read the first input sequence.

Step 3: Read the second impulse sequence.

Step 4: Plot the input sequences with x-label and y-label with suitable title. 

Step 5: Perform convolution for both the sequences using conv2() function.

Step 6: Plot the sequence with x-label and y-label with suitable title

Step 7: Terminate the program.

## PROGRAM: 
```
clc;
clear all;
close all;
a=input('enter the starting x(n)');
x=input('enter the x(n) sequence');
n=a:1:length(x)+a-1;
figure(1);
stem(n,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');
b=input('enter the starting h(n)');
y=input('enter the h(n) sequence');
m=b:1:length(y)+b-1;
figure(2);
stem(m,y);
xlabel('time');
ylabel('amplitude');
title('impulse response');
z=conv2(x,y);
nl=a+b:1:length(z)+a+b-1;
figure(3);
stem(nl,z);
xlabel('time');
ylabel('amplitude');
title('linear convolution');
```
## OUTPUT:
<img width="727" height="644" alt="Screenshot 2026-02-09 202711" src="https://github.com/user-attachments/assets/de42ca67-e96a-4e1a-8991-70ed27cc197c" />
<img width="706" height="641" alt="Screenshot 2026-02-10 075241" src="https://github.com/user-attachments/assets/73e8178e-0434-46d5-bdc8-eb50b815200e" />
<img width="713" height="658" alt="Screenshot 2026-02-10 075257" src="https://github.com/user-attachments/assets/5ec4a07d-07b7-47ed-89c9-7653ed9833ac" />
## RESULT:
<img width="1280" height="721" alt="image" src="https://github.com/user-attachments/assets/33d30842-8c0f-458f-87c4-57d64241e25d" />


