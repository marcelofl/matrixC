# matrixC
include <stdio.h>
#include <stdlib.h>

int main()
{
   float matA[2][2], matB[2][2], matC[2][2], Aux=0;
   int i, j, X;
   printf("\n\n");
   printf("Produto de duas matrizes 2X2 \n\n");
   for (i = 0; i < 2; i++){
      for (j = 0; j < 2; j++){
         printf("Digite o valor de matA[%d][%d]: ",i,j);
          scanf("%f]",&matA[i][j]);
    }
   }
 printf("\n\n");
   for (i = 0; i < 2; i++){
     for (j = 0; j < 2; j++){
         printf("Digite o valor de matB[%d][%d]: ",i,j);
          scanf("%f]",&matB[i][j]);
     }
   }
  printf("Matriz A \n\n");
  for(i=0; i<2; i++){
     for(j=0; j<2; j++){
         printf("%6.f", matA[i][j]);
     }
         printf("\n\n");
  }
 printf("Matriz B \n\n");
  for(i=0; i<2; i++){
     for(j=0; j<2; j++){
         printf("%6.f", matB[i][j]);
     }
         printf("\n\n");
  }
  for(i=0; i<2; i++){
     for(j=0; j<2; j++){
         matC[i][j]=0;
             for(X=0; X<2; X++){
               Aux += matA[i][X] * matB[X][j];
             }
                  matC[i][j]=Aux;
                  Aux=0;
      }
  }
  printf("Matriz C \n\n");
    for(i=0; i<2; i++){
       for(j=0; j<2; j++){
           printf("%6.f", matC[i][j]);
       }
           printf("\n\n");
    }
  system("pause");
  return 0;
}
