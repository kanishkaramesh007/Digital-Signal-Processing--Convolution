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
% KANISHKA R S [212223050026]

clc; % clear screen
clear all; % clear screen
close all; % close all figure windows

% input sequence
% 𝑥[𝑛]={2.7,3.5,2,2, −1, 4, 9, −3} ℎ[𝑛] = {3, 2.7,3.5,2,−4,1,1}

a = input("enter the starting x(n)");
x = input("enter the x(n) sequence");
n = a:1:length(x)+a-1;
figure(1);
stem(n,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');

%impulse sequence

b= input('enter the starting h(n)');
y = input('enter the h(n) sequence');
m = b:1:length(y)+b-1;
figure(2);
stem(m,y);
xlabel('time');
ylabel('amplitude');
title('impulse response');

%linear convolution

z = conv2(x,y);
n1 = a+b:1:length(z)+a+b-1;
figure(3);
stem(n1,z);
xlabel('time');
ylabel('amplitude');
title('linear convolution');
```

## OUTPUT:
![WhatsApp Image 2026-04-02 at 6 27 27 PM](https://github.com/user-attachments/assets/bf50bafd-86f7-4b81-8882-cc7d8163bb4d)
![WhatsApp Image 2026-04-02 at 6 27 47 PM](https://github.com/user-attachments/assets/35812d18-4e4b-4264-859f-d4215b17fe69)
![WhatsApp Image 2026-04-02 at 6 28 13 PM](https://github.com/user-attachments/assets/57876144-35dc-4c24-8219-96556e6a362a)



## RESULT:
![WhatsApp Image 2026-04-02 at 6 21 11 PM](https://github.com/user-attachments/assets/f9f860ed-44c5-4da1-a31f-237abb74a431)
