# Resposta-Desafio-Target-Sistemas

1 - 91

2 -

```
#include <stdio.h>

int main() 
{
    
    int num;
    
    printf("insira numero: ");
    scanf("%i", &num);
    
    int fib[3];
    fib[0] = 0;
    fib[1] = 1;
    
    while(fib[2] < num)
    {
        fib[2] = fib[0] + fib[1];
        fib[0] = fib[1];
        fib[1] = fib[2];
    }
    if (fib[2] == num)
    {
        printf("O numero PERTENCE a sequencia");
    }
    else {
         printf("O numero NAO pertence a sequencia");
    }
}
```

3 a) 9
b) 128
c) 49
d) 100
e) 13
f) 200

4 - 

5 - 
```
#include <stdio.h>
#include <string.h>

int main() {
    
    char string[10];
    char stringrev[10];
    
    printf("insira palavra: ");
    scanf("%s",&string);
    
    for (int i = 0; i < strlen(string); i++)
    {
        stringrev[i] = string[strlen(string) - 1 - i];
    }
    printf("%s", stringrev);
}
```
