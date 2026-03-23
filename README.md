# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 
# Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside the main() function, use printf() to display each literal along with its size in bytes using sizeof() :
  
   3.1 Integer literal (e.g., 10) using `%d`
   
   3.2 Float literal (e.g., 3.14) using `%f`
   
   3.3 Character literal (e.g., 'A') using `%c`
   
   3.4 String literal (e.g., "Hello C") using `%s`
   
### Step 4: 
   Stop
# Program:
```
#include<stdio.h>
int main(){
    float math,science,english,average;
    printf("Enter marks for Math, Science and English: ");
    scanf("%f %f %f",&math,&science,&english);
    average=(math+science+english)/3.0f;
    if(average>=90.0f)
        printf("Grade A\n");
    else if(average>=75.0f)
        printf("Grade B\n");
    else if(average>=50.0f)
        printf("Grade C\n");
    else
        printf("Grade F\n");
    return 0;
}
```
# Output:
<img width="983" height="1020" alt="image" src="https://github.com/user-attachments/assets/caddf3fa-7acb-4712-9225-95f5dc9e981a" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 
# Aim:
  To build a C program that demonstrates the use of macro constants and constant variables.
# Algorithm:
### Step 1:
  Start  
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Define a macro constant `PI` with value `3.14159` using `#define`.
### Step 4: 
   Inside `main()`:
   
   4.1 Declare a constant integer variable `DAYS`
   
   4.2 Initialize it with the value `7`
   
### Step 5:  
  Use `printf()` to display the values of `PI` and `DAYS`.     
### Step 6:  
  Stop
# Program:
```
#include<stdio.h>
int main(){
    int number=15,i;
    for(i=1;i<=10;i++){
        printf("%d x %d = %d\n",number,i,number*i);
    }
    return 0;
}
```
# Output:
<img width="983" height="1020" alt="image" src="https://github.com/user-attachments/assets/b2bc4f40-9b30-4785-829c-37c03bf9de1b" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 
# Aim:
  To build a C program that declares variables of various data types—integer, float, double, and character—initializes them, and prints their values on the screen.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside main(), declare and initialize variables of types int, float, double, and char.
### Step 4: 
   Display their values using printf().
### Step 5:    
   Stop
# Program:
```
#include<stdio.h>
int main(){
    int n, i = 2, f = 0;
    scanf("%d", &n);
    while(i <= n - 1){
        if(n % i == 0){
            f = 1;
            break;
        }
        i++;
    }
    if(f == 0 && n > 1)
        printf("%d is a prime number.\n", n);
    else
        printf("%d is not a prime number.\n", n);
    return 0;
}

```
# Output:
<img width="983" height="1020" alt="image" src="https://github.com/user-attachments/assets/82c0b132-997e-4130-8014-83b788e6a19a" />

# Result: 

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date : 
# Aim:
  To build a C program that takes two integers as input and demonstrates the arithmetic and bitwise operations, displaying the results of each operation.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare two integer variables a and b.
### Step 4: 
   Prompt the user to enter two integers and read the input using scanf().
### Step 5:    
   Perform arithmetic operations on a and b:
   #### Sum (a + b)
   #### Difference (a - b)
   #### Product (a * b)
   #### Quotient (a / b)
   #### Remainder (a % b)
### Step 6: 
  Perform bitwise operations on a and b:
  #### AND (a &amp; b)
  #### OR (a | b)
  #### XOR (a ^ b)
  #### Left shift (a << b)
  #### Right shift (a >> b)
  #### Bitwise NOT of a (~a) and b (~b)
### Step 7:   
  Display the results of all operations using printf().
### Step 8:   
  Stop
# Program:
```
int main(){
    int n, i, j, k;
    scanf("%d", &n);
    
    for(i = 1; i <= n; i++){
        for(j = i; j <= n; j++){
            if(i == 1 || j == i)
                printf("%d", j);
            else
                printf(" ");
        }
        k = j - 2;
        for(j = 1; j <= i - 1; j++){
            if(i == n || j == i - 1)
                printf("%d", k);
            else
                printf(" ");
            k--;
        }
        printf("\n");
    }
    
    return 0;
}
```
# Output:
<img width="983" height="1020" alt="image" src="https://github.com/user-attachments/assets/31113992-6b62-401e-8888-1d89b6913882" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 
# Aim:
  To develop and implement a C program that classifies a character as a vowel, consonant, digit, or special symbol using the ternary operator.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Input a character ch from the user.
### Step 4: 
   Check if ch is a digit ('0' to '9').
   
   If true → Print "Digit" → Go to Step 8.
   
   If false → Go to Step 5.
   
### Step 5:    
   Check if ch is an alphabet letter ('A' - 'Z' or 'a' – 'z').
   
   If true → Go to Step 6.
   
   If false → Go to Step 7.
   
### Step 6: 
   Check if ch is a vowel (a, e, i, o, u or A, E, I, O, U).
   
   If true → Print "Vowel" → Go to Step 8.
   
   If false → Print "Consonant" → Go to Step 8.
   
### Step 7:   
   Print "Special Symbol".
### Step 8:   
  Stop
# Program:
```
#include<stdio.h>

int main(){
    int i, j;
    printf("0\n");
    for(i = 7; i >= 1; i--){
        for(j = i; j <= 7; j++)
            printf("%d ", j);
        printf("0 ");
        for(j = 7; j >= i; j--)
            printf("%d ", j);
        printf("\n");
    }
    return 0;
}
```
# Output:
<img width="983" height="1020" alt="image" src="https://github.com/user-attachments/assets/b8c1b89d-b1f3-4cd7-8786-aed762d1c104" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


