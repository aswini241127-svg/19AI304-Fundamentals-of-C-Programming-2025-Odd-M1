# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 27/01/26
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
#include <stdio.h>

int main() {
    int intLiteral = 10;
    float floatLiteral = 3.14;
    char charLiteral = 'A';
    char stringLiteral[] = "Hello C";

    printf("Integer literal: %d, Size: %lu bytes\n", intLiteral, sizeof(intLiteral));
    printf("Float literal: %f, Size: %lu bytes\n", floatLiteral, sizeof(floatLiteral));
    printf("Character literal: %c, Size: %lu bytes\n", charLiteral, sizeof(charLiteral));
    printf("String literal: %s, Size: %lu bytes\n", stringLiteral, sizeof(stringLiteral));

    return 0;
}
```
# Output:

 <img width="821" height="363" alt="530353376-e770a197-ec38-4bfc-bc79-7383d53e2c7a" src="https://github.com/user-attachments/assets/85e3fb78-a480-4f90-8126-35d15d348324" />
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
#include <stdio.h>
#define PI 3.14159
int main() {
    const int DAYS = 7;

    printf("Value of macro constant PI: %f\n", PI);
    printf("Value of constant variable DAYS: %d\n", DAYS);

    return 0;
}
```

# Output:
<img width="834" height="340" alt="530353580-71600d94-790b-4aeb-9832-f359ec2b12ea" src="https://github.com/user-attachments/assets/8d12e841-6789-4141-9234-04edf7eb2908" />

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
#include <stdio.h>
int main() {
    int intVar = 25;
    float floatVar = 5.75;
    double doubleVar = 19.99;
    char charVar = 'G';
    printf("Integer value: %d\n", intVar);
    printf("Float value: %f\n", floatVar);
    printf("Double value: %lf\n", doubleVar);
    printf("Character value: %c\n", charVar);
    return 0;
}
```
# Output:
<img width="820" height="309" alt="530353691-f9cd545a-b9dc-4fd8-9c99-86543039ac4a" src="https://github.com/user-attachments/assets/ae7e3553-7382-4b19-807b-2d3d10f9d8e3" />

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
#include <stdio.h>
int main() {
    int a, b;
    printf("Enter two integers: ");
    scanf("%d %d", &a, &b);
    printf("Arithmetic Operations:\n");
    printf("Sum (a + b) = %d\n", a + b);
    printf("Difference (a - b) = %d\n", a - b);
    printf("Product (a * b) = %d\n", a * b);
    if(b != 0) {
        printf("Quotient (a / b) = %d\n", a / b);
        printf("Remainder (a %% b) = %d\n", a % b);
    } else {
        printf("Division by zero is not allowed.\n");
    }
    printf("\nBitwise Operations:\n");
    printf("AND (a & b) = %d\n", a & b);
    printf("OR (a | b) = %d\n", a | b);
    printf("XOR (a ^ b) = %d\n", a ^ b);
    printf("Left shift (a << b) = %d\n", a << b);
    printf("Right shift (a >> b) = %d\n", a >> b);
    printf("Bitwise NOT of a (~a) = %d\n", ~a);
    printf("Bitwise NOT of b (~b) = %d\n", ~b);
    return 0;
}
```

# Output:
<img width="819" height="564" alt="530353806-c961a8f4-20ba-4cda-bdd8-dcf421a81cdc" src="https://github.com/user-attachments/assets/7f9fe4fd-f55b-46ae-9743-41a919e863db" />

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
    char ch;
    printf("Enter a character: ");
    scanf("%c",&ch);
    (ch>='0' && ch<='9')?printf("Digit\n"):
    ((ch>='A' && ch<='Z')||(ch>='a' && ch<='z'))?
    ((ch=='A'||ch=='E'||ch=='I'||ch=='O'||ch=='U'||ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u')?printf("Vowel\n"):printf("Consonant\n"))
    :printf("Special Symbol\n");
    return 0;
}
```
# Output:
<img width="820" height="112" alt="530353901-44200bc0-b252-4daa-bc01-07eb4f15c22e" src="https://github.com/user-attachments/assets/dcd9025d-5a13-476c-a23f-397357fd558d" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


