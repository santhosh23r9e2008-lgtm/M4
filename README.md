# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main() {
    int a = 44, b = 3, result;
    result = a << b;   
    printf("Result after left shifting %d by %d positions: %d\n", a, b, result);
    return 0;
}

```
## OUTPUT
<img width="1625" height="749" alt="Screenshot 2025-10-22 103927" src="https://github.com/user-attachments/assets/34645f3c-183e-470f-bab2-8fd655a6f3ed" />



## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main() {
    int num1, num2;
    printf("Enter first number: ");
    scanf("%d", &num1);
    printf("Enter second number: ");
    scanf("%d", &num2);
    if(num1 == num2)
        printf("Both numbers are equal.\n");
    else
        printf("Both numbers are not equal.\n");
    return 0;
}

```
## OUTPUT
<img width="1622" height="741" alt="Screenshot 2025-10-22 104114" src="https://github.com/user-attachments/assets/5b35601e-372f-47f2-9f3b-a2cba75a2669" />
           
## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <ctype.h>
int main() {
    char str[100];
    int i;
    printf("Enter a string: ");
    fgets(str,sizeof(str),stdin;  
    for(i = 0; str[i] != '\0'; i++) {
        str[i] = tolower(str[i]);
    }
    printf("String in lowercase: %s\n", str);
    return 0;
}

```
## OUTPUT
<img width="1619" height="718" alt="Screenshot 2025-10-22 104417" src="https://github.com/user-attachments/assets/ddba99d0-f4ef-45d9-b0d4-11b4acec814c" />


## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main() {
    char str[200];
    int i = 0, count = 1;
    printf("Enter a string: ");
    fgets(str, sizeof(str),stdin);
    do {
        if (str[i] == ' ' && str[i + 1] != ' ' && str[i + 1] != '\0')
            count++;
        i++;
    } while (str[i] != '\0');
    printf("Total number of words: %d\n", count);
    return 0;
}

```
## OUTPUT
<img width="1627" height="754" alt="Screenshot 2025-10-22 104919" src="https://github.com/user-attachments/assets/5dfe5f85-ecfc-44cf-aff2-172fb410c979" />


## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
Step 1: Start the program.
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable
             flag and initialize it to 0, and i for indexing.      
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
Step 5: Start comparing characters of both strings from index i = 0.
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
Step 7: After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
Step 8: End the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    char c1[100], c2[100];
    int i = 0, flag = 0;
    printf("Enter first string: ");
    scanf("%[^\n]", c1);
    printf("Enter second string: ");
    scanf("%s", c2);
    while(c1[i] != '\0' && c2[i] != '\0') {
        if(c1[i] != c2[i]) {
            flag = 1;
            break; 
        }
        i++;
    }
    if(flag == 0) {
        printf("Strings are same\n");
    } else {
        printf("Strings are not same\n");
    }
    return 0;
}

```
## OUTPUT
 <img width="1615" height="774" alt="Screenshot 2025-10-22 110033" src="https://github.com/user-attachments/assets/ba6cdbde-f782-43c0-b214-06993625b5fa" />

## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

