# EX-NO-6-Pseudo-Random-Number
## NAME: M BALASURIYA
## REG.NO: 212224240021

# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM:
Start the program and import the required libraries.<br>
Seed the random number generator using the current time(i.e) rand(time(0));<br>
Get the number of randon number to generate.<br>
Pass the value for number of iterations and print the numbers.<br>
End the program.

# PROGRAM:
```c
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() 
{
    int count, min, max;
    printf("Enter the number of random numbers to generate: ");
    scanf("%d", &count);
    printf("Enter the minimum value: ");
    
    scanf("%d", &min);
    printf("Enter the maximum value: ");
    scanf("%d", &max);
    srand(time(NULL));
    printf("Pseudorandom numbers:\n");   
    for (int i = 0; i < count; i++) 
    {
        int random_number = (rand() % (max - min + 1)) + min;
        printf("%d\n", random_number);
    }
    return 0;
}
```

# OUTPUT:
<img width="1248" height="534" alt="image" src="https://github.com/user-attachments/assets/bc459e10-0c1d-4962-8c91-887d11c16b21" />


# RESULT:
Hence the implementation of pseudorandom number generation has successfully created using standard library.
