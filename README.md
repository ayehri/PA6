# Programming Assignment 6

## Intended Learning Outcomes:
1. To be able to differentiate a script file from a function file.
2. To be able to apply and use the different codes and built-in functions in creating a MATLAB script
files and function files.

# Problem 1
<img width="712" height="156" alt="image" src="https://github.com/user-attachments/assets/d1c24b36-b751-4de6-9a45-9826b551e5bf" />

### Code:
<img width="805" height="299" alt="image" src="https://github.com/user-attachments/assets/7300621e-4f38-4dd3-839e-84efd55dcb3b" />

### Output:
<img width="300" height="123" alt="image" src="https://github.com/user-attachments/assets/0bb5bd4f-ccec-4e24-8e78-d5f7d61ae9a0" />

### Explanation:
- classifyconic: Function name
- d = B^2 - 4*A*C: The formula for calculating the discrimant
- if d == 0: Checks if the discrimant is equal to zero
- shape = 'Parabola': If d is equal to zero, then the shape is a Parabola
- elseif d<0: Checks if the discrimant is less than zero
- shape = 'Ellipse': If the discrimant is less than zero or negative, then it is an Ellipse
- else: The last condition. The discrimant should now be a positive number
- shape = 'Hyperbola': if d is positive, then it is a Hyperbola
- end: To end the statements

# Problem 2
<img width="711" height="90" alt="image" src="https://github.com/user-attachments/assets/4db0b78a-17c9-48f8-83a9-ce2357c3a9e5" />

### Code:
<img width="419" height="204" alt="image" src="https://github.com/user-attachments/assets/e21f44a9-b049-42c5-83b4-7cea12618e43" />

### Output:
<img width="350" height="70" alt="image" src="https://github.com/user-attachments/assets/d860c8c2-1b7a-43cc-bdbd-5608fea01cf3" />
<img width="237" height="38" alt="image" src="https://github.com/user-attachments/assets/fd32c67c-4243-4766-be9c-ef32e56708dc" />

### Explanation:
- a = input('Please enter the value of side a: '): Prompts the user to input the value of side a. It will also be stored in variable a
- b = input('Please enter the value of side b: '): Prompts the user to input the value of side b. It will also be stored in variable b
- C = input('Please enter the value of side C: '): Prompts the user to input the value of side C. It will also be stored in variable c
- c = sqrt(a^2 + b^2 - 2*a*b*cosd(C)): Law of cosines formula to calculate the length of side C.
- fprintf('The value of side c is %.2f units.', c): Prints the value of side c with 2 decimal places.
  
# Problem 3: With loop
<img width="707" height="147" alt="image" src="https://github.com/user-attachments/assets/5d3cd244-83fa-49ac-bb45-9db92ce5b958" />

### Code:
<img width="553" height="314" alt="image" src="https://github.com/user-attachments/assets/d74453ce-0b44-4c6d-bde7-bfcf6a9311e5" />

### Output:
<img width="557" height="218" alt="image" src="https://github.com/user-attachments/assets/850b84c0-98dc-4b8c-9e04-99ff2dddbfa9" />

### Explanation:
- isolate: Function name 
- function[evenvector, oddvector] = isolate(x): This defines a function named isolate and returns two outputs which is the evenvector and the oddvector.
- evenvector =[]: Where all even numbers will be stored.
- oddvector = []: Where all odd vectors will be stored.
- for i = 1:length(x): A for loop with i as an index
- if mod(x(i),2) == 0: Checks if the number is even. It also returns the remainder when dividing by 2.
- evenvector(end+1) = x(i): if it's even, then it is added to the evenvector.
- else: else statement wherein if the number is not even, it  must be odd.
- oddvectors(end+1)=x(i): if it's odd, then it is added to the oddvector.
- end: To end the if-else statement
- end: The final end. Markts the end of the for-loop and the function.

# Problem 3: Without Loop
<img width="707" height="147" alt="image" src="https://github.com/user-attachments/assets/5d3cd244-83fa-49ac-bb45-9db92ce5b958" />

### Code:
<img width="613" height="222" alt="image" src="https://github.com/user-attachments/assets/d445fadb-8139-4062-a699-13f7b4253e9e" />

### Output:
<img width="480" height="228" alt="image" src="https://github.com/user-attachments/assets/b373cb36-9181-436c-8008-b27d3eb9f2f5" />

### Explanation:
- isolate2: The function name. I named it isolate2 because I can't rename the file to isolate again since I already used it for the previous code with loop.
- function[evenvector, oddvector] = isolate2(x): Defines a function named isolate2 that accepts one input vector and returns two output vectors: evenvector and oddvector
- evenvector = x(mod(x,2)==0): identifies all even numbers in x and stores them in evenvector.
- oddvector = x(mod(x,2)==1): identifies the odd numbers in x and stores them in oddvector.
- end: Marks the end of the function.

## Conclusion
In this programming assignment, I learned how to use MATLAB more effectively, including working through the Command Window and creating script and function files. In Problem 1, I created a function that classifies a conic section as a parabola, ellipse, or hyperbola by calculating its discriminant. In Problem 2, I applied the Law of Cosines to determine the length of a side in an oblique triangle. In Problem 3, I separated a vector into two groups: even numbers and odd numbers. I accomplished this using two methods, one with a loop and one without a loop, and both methods produced the same results. Overall, this assignment helped strengthen my understanding of writing functions, using conditional statements, and working with vectors in MATLAB.
