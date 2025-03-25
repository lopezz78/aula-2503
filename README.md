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


/*3. Ler um vetor de inteiros 10 posições. Escrever a seguir o
valor e a posição do maior e menor elementos lidos.*/

#include <stdlib.h>
#include <stdio.h>
#include <locale.h>
#define tam 5


int main()
{
    int A[tam], i, maior, menor, posicaomaior, posicaomenor;
     printf("A[%d]= ",0);
    scanf("%d", &A[0]);
    maior=A[0];
    menor=A[0];
    posicaomaior = 0;
    posicaomenor= 0;
    for( i=1 ; i<tam ; i++ )
    {
        printf("A[%d]= ",i);
        scanf("%d", &A[i]);

        if (A[i]>maior)
        {
            maior = A[i];
            posicaomaior = i;

        }
        else
        {
            if ( A[i] < menor)
            {
                menor = A[i];
                posicaomenor= i;
            }
        }


    }


        printf("\n\tmaior = %d, posicao numero %d", maior, posicaomaior );
        printf("\n\tmenor = %d, posicao numero %d", menor, posicaomenor );

}
