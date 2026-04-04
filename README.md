# Digital-Signal-Processing--Correlation
## AIM:
To generate discrete auto correlation and cross correlation of signals using MATLAB.
## APPARATUS REQUIRED:
MATLAB R2012.
## ALGORITHM:
Step 1: Open matlab. Write the program.

Step 2: Read the input sequence 1 and input sequence 2 sequence.

Step 3: Perform auto correlation and cross correlation for both the sequences. 

Step 4: Plot the output sequence with x-label and y-label with suitable title.

Step 5: Terminate the program.


## PROGRAM: 
```
clc; % clear screen
clear all; % clear screen
close all; % close all figure windows
% INPUT SIGNAL-1
a=input('enter the starting x(n)');
x=input('Enter the x(n) sequence');
n=a:1:length(x)+a-1;
figure(1)
stem(n,x)
xlabel('Time')
ylabel('Amplitude')
title('Input Signal-1')
% INPUT SIGNAL 2
b=input('enter the starting y(n)');
y=input('Enter the y(n) sequence');
m=input('enter the ending y(n)');
n1=b:1:length(y)+b-1;
figure(2)
stem(n1,y)
xlabel('time')
ylabel('amplitude')
title('input signal-2')
%discrete auto correlated signal 
out1=xcorr(x,x)
n2=a-m:1:length(out1)+a-m-1;
figure(3)
stem(n2,out1)
xlabel('time')
ylabel('amplitude')
title('discrete auto correlated waveform')
%discrete cross correlated signal
out2=xcorr(x,y)
n3=a-m:1:length(out2)+a-m-1;
figure(4)
stem(n3,out2)
xlabel('time')
ylabel('amplitude')
title('discrete cross correlated waveform')
```

## OUTPUT:

<img width="696" height="624" alt="image" src="https://github.com/user-attachments/assets/72cf7f92-fa65-4a93-a64a-56e82c8584d9" />

<img width="703" height="638" alt="Screenshot 2026-04-04 133342" src="https://github.com/user-attachments/assets/f20d63ff-e5f2-49c7-ab18-9d37d120dd24" />

<img width="704" height="622" alt="Screenshot 2026-04-04 133355" src="https://github.com/user-attachments/assets/43c8e8c8-bfdb-44c8-ad4f-3a62ea5e6fc8" />

<img width="696" height="624" alt="Screenshot 2026-04-04 133405" src="https://github.com/user-attachments/assets/5be76747-1b68-4923-b88e-727bf42e8357" />


## RESULT:
<img width="846" height="1372" alt="image" src="https://github.com/user-attachments/assets/4d9d1fd7-5ccc-4961-ade4-0aaf921117da" />

