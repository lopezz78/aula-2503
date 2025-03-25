# aula-2503
/*Elaborar um programa que leia um vetor de no máximo 15
elementos inteiros. O programa deverá imprimir o vetor e
informar quantos números são maiores que 30.*/

#include <stdlib.h>
#include <stdio.h>
#include <locale.h>
#define tam 15

int main()
{
    int A[15], i;

    for( i=0 ; i<tam ; i++ )
    {
        scanf("%d", &A[i]);
    }
        for ( i=0 ; i<tam ; i++)
        {

            printf("%d ", A[i]);
            if (i !=14)
                printf(", ");
            else
                printf(". ");

        }

            for ( i=0 ; i<tam ; i++)
            {
                if (A[i] > 30)
                    printf("%d", A[i]);
            }


}
