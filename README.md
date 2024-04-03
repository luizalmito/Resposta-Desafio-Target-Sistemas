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


3 - a) 9

b) 128

c) 49

d) 100

e) 13

f) 200



4 - Liga-se o interruptor 1 por 5 minutos, desliga, e liga o 2. verificando em uma das salas, se houver uma lâmpada acesa, pertencerá ao interruptor 2, se apagada e quente ao 1, e se fria, ao 3.
Liga-se um dos outros 2 interruptores, e verifica-se em uma das outras salas, se a lâmpada estiver acesa, pertence àquele interruptor ligado, se não ao outro. E por lógica, a ultima lâmpada pertence ao último interruptor.


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
