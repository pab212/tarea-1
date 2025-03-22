# tarea-1
#include <stdio.h>
#include <stdlib.h>

int main () {
    char *precio_total []={"4","1","0","21","3","313313"};
    char *precio[]= {"3","2","2","8","8"};
    char *cantidad_pizzas[] = {"2", "3", "4", "1", "1"};
    

    int cantidad3 = sizeof(precio_total) / sizeof(precio_total[0]);
    int numeros3[cantidad3];



    int cantidad2 = sizeof(precio) / sizeof(precio[0]);
    int numeros2[cantidad2];
    
    
    int cantidad = sizeof(cantidad_pizzas) / sizeof(cantidad_pizzas[0]);
    int numeros[cantidad];
    
    for (int i = 0; i < cantidad; ++i) {
        numeros[i] = atoi(cantidad_pizzas[i]); // Convertir cada cadena a entero
        printf("El número convertido %d es: %d\n", i + 1, numeros[i]);
    }
    

    for (int i = 0; i < cantidad2; ++i) {
        numeros2[i] = atoi(precio[i]); // Convertir cada cadena a entero
        printf("El número convertido %d es: %d\n", i + 1, numeros2[i]);
    }


    for (int i = 0; i < cantidad3; ++i) {
        numeros3[i] = atoi(precio_total[i]); // Convertir cada cadena a entero
        printf("El número convertido %d es: %d\n", i + 1, numeros3[i]);
    }

    
    
    return 0;    
}




