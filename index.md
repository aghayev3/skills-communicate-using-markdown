# Github Markdown Practice

### Hey everyone, nothing crazy, just practicing reading GitHub courses and working on assignments :)


![Battle of Verdun, 1916](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e6/Bataille_de_Verdun_1916.jpg/640px-Bataille_de_Verdun_1916.jpg)

Some bad C code

```c
#include <stdio.h> 
#include <string.h> 


void main() { // 'main' should return int
    int n; 
    printf("Enter a number: "); 
    scanf("%f", &n); // Using %f for an int variable

    char str[5]; 
    printf("Enter a string: "); 
    gets(str); // 'gets' is dangerous and deprecated

    if (n = 10) { // Using '=' instead of '=='
        printf("You entered 10!\n");
    }

    // Array out of bounds
    char arr[3] = {'a', 'b', 'c'};
    printf("Fourth element: %c\n", arr[3]);

    // Uninitialized pointer
    int *ptr;
    printf("Pointer value: %d\n", *ptr);

    // Memory leak and undefined behavior
    int *leaky_ptr = malloc(sizeof(int) * 10); 
    leaky_ptr[10] = 100; // Out-of-bounds memory write
    printf("Leaky value: %d\n", leaky_ptr[10]);

    // Dangerous string copy
    char dest[5];
    strcpy(dest, "This is way too long!"); // No bounds check

    // Infinite recursion
    main();

    // Missing free and return
}
```
