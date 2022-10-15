# ESTRUTURA-DE-DADOS2

60° RESPOSTA

#include <stdio.h>
#include <stdlib.h>

vetor vazio()
{

   int A[] = { 1,0,5,-2,-5,7 };
 int i,t;

   t = A[0] + A[1] + A[5];

   printf("A soma dos vetores eh %i\n", t);
 printf ("%d%d%d\n------------------------\n", A[0], A[1], A[5]);
   A[4] = 100;

 para (i=0; i<=5; i++){
 printf ("%d\n", A[i]);
   }
}

61° RESPOSTA
#include <stdio.h>
#include <stdlib.h>

int principal()
{
   int i, num[6];
 printf ("Digite 6 numeros inteiros.\n");

 para(i=0; i<6; i++) {
    printf("Digite o %d valor: ", (i+1));
    scanf("%d", &num[i]);
   }

 printf ("Resultado:\n");
 para(i=5; i>=0; i--) {
 printf ("%d\n", num[i]);
   }
 retorno 0;
}

62° RESPOSTA
#include <stdio.h>

int principal(){

 int i;

 flutuar qtdNum[10], numQuad[10];
   printf("Digite os 10 números que serão feitos o quadrado: \n");

 para(i=0; i<10;i++){
   scanf("%f",&qtdNum[i]);
}
for(i=0; i<=9; i++){ //cálculo do quadrado do número

  numQuad[i] = qtdNum[i] * qtdNum[i];
}
printf("\nNúmeros digitados:");

for(i=0; i<=9; i++){ // aqui mostra seus números digitados

    printf("%2.f ",qtdNum[i]);
}
printf("\nNúmeros quadrados: ");

for(i=0; i<=9; i++){//aqui mostra o quadrado dos números
  printf("%.2f ",numQuad[i]);
}

return 0;

}

63° RESPOSTA
#include <stdio.h>
#include <stdlib.h>
#include <locale.h>

int main()
{

    setlocale(LC_ALL, "Portuguese"); 
    int vet[8],x,y,i,soma;
    for(i=1;i<=8;i++)
{
        printf("Digite o %i vetor:",i);
            scanf("%d",&vet[i]); 
}
             x=vet[5]; 
             y=vet[7]; 
        printf("O valor do vetor X e: %i\n",x);
        printf("O valor do vetor Y e: %i\n",y);
            soma=vet[5]+vet[7];

        printf("\n A soma de X e Y e: %i",soma);
return 0;
}

64° RESPOSTA
#include<stdio.h>
#include<conio.h>

int main() {

int numeros[10],par=0,contador=0;

for(int i=0;i<10;i++){
    printf("Informe um valor inteiro:");
    scanf("%d",&numeros[i]);
}
for(int i=0;i<10;i++){
    if(numeros[i]%2==0){
    contador=contador+1;
    }
}
    printf("O total de numeros pares e:%d",contador);

    return 0;
}


65° RESPOSTA
#include <stdio.h>

int main()
{
    int n = 4;
    int C[10];
    printf("[%d de %d] Numero: ", 1,n);
    if( scanf("%d", &C[0]) !=1 ) return -1; 
    int maior = C[0];
    int menor = maior;

    for (int i=1; i<n; i+=1)
    {
        printf("[%d de %d] Numero: ", 1+i, n);
        if (scanf("%d", &C[i]) != 1) return -1; 
        if (menor > C[i]) menor = C[i];
            else if (maior < C[i]) maior = C[i];
    }
    printf("\
o menor e %d\n\
o maior e %d\n",
        menor, maior);
    return 0;
}

66° RESPOSTA
#include <stdio.h>
#include <stdlib.h>

int main(){

   int a, maior=0, menor=0;
   int valor[10];

   printf("digite 10 valores");
   printf("\n");

   for (a=0;a<10;a++){

     printf("valor %d : ", a+1);
     scanf("%d", &valor[a]);

     if (a==0){
          maior=valor[a];
          if(valor[a]>maior){
              maior=valor[a];
         }
     }
   }
   printf("\no maior valor é %d\n", maior);

   return 0;

}

67° RESPOSTA
#include <stdio.h>
#include <stdlib.h>

int main() {

    int i, opcao;
    float vetor[6];

    for(i = 0; i < 6; i++){
        printf("Digite o valor da posicao %d: ", i);
        scanf("%f", &vetor[i]);
    }

    do{
        printf("\n0 - Fizalizar\n1 - Imprimir vetor\n2 - Imp. vetor invertido\n");
        scanf("%d", &opcao);

        switch(opcao){
        case 0:
            printf("Finalizando...\n");
            break;
        case 1:
            for(i = 0; i < 10; i++){
                printf("%.2f ", vetor[i]);
            }
            printf("\n");
            break;
        case 2:
            for(i = 9; i >= 0; i--){
                printf("%.2f ", vetor[i]);
            }
            printf("\n");
            break;
        default:
            printf("Opcao invaalida!\n");
        }

    }while(opcao != 0);

    return 0;
}

}

68° RESPOSTA
#include <stdio.h>
#include <stdlib.h>

int main() {

    int i, opcao;
    float vetor[6];

    for(i = 0; i < 6; i++){
        printf("Digite o valor da posicao %d: ", i);
        scanf("%f", &vetor[i]);
    }

    do{
        printf("\n0 - Fizalizar\n1 - Imprimir vetor\n2 - Imp. vetor invertido\n");
        scanf("%d", &opcao);

        switch(opcao){
        case 0:
            printf("Finalizando...\n");
            break;
        case 1:
            for(i = 0; i < 10; i++){
                printf("%.2f ", vetor[i]);
            }
            printf("\n");
            break;
        case 2:
            for(i = 9; i >= 0; i--){
                printf("%.2f ", vetor[i]);
            }
            printf("\n");
            break;
        default:
            printf("Opcao invaalida!\n");
        }

    }while(opcao != 0);

    return 0;
}
}

69° RESPOSTA
#include <stdio.h>

int main(){

int notas[15], i,total=0, media;

for(i=0;i<15;i++){

 scanf("%d", &notas[i]);
}
for(i=0;i<15;i++){

 total = total + notas[i];
}
media = (total/15);
printf("A media geral e: %d", media);

return 0;

}

70° RESPOSTA
#include <stdio.h>
#include <stdlib.h>

int main(){

 int num[10], count = 0, soma = 0;

 printf("Informe 10 numeros reais:\n");

 for(int i = 0; i < 10; i++){
 
   printf("[%i]: ", i+1);
   scanf("%d", &num[i]);

   if(num[i] < 0){
     count++;
   }
   if(num[i] > 0){
    soma = soma + num[i];
   }
 }
 printf("\n\n%d numeros negativos.\nSoma dos numeros positivos = %d.\n", count, soma);

return 0;

}

71° RESPOSTA
#include <stdio.h>
#include <stdlib.h>

int main() {
    int valor[5],i,maior,menor,maiorPosicao,menorPosicao;
    for(i=0; i<5; i++) {
        printf(" Entre com um numero: ");
        scanf("%d",&valor[i]);
        if(i == 0) {
            maior = valor[i];
            menor = valor[i];
            maiorPosicao = i;
            menorPosicao = i;
        }
        if(valor[i] > maior) { 
            maior = valor[i];
            maiorPosicao = i;
        }
        if(valor[i] < menor) {
            menor = valor[i]; //e aqui afaltou um ;
            menorPosicao = i;
        }
    }
    printf("\n Maior valor: %d  Posicao %d",maior,maiorPosicao);
    printf("\n Menor valor: %d  Posicao %d",menor,menorPosicao);
    system("pause");
}

72° RESPOSTA
#include <stdio.h>
#include <stdlib.h>

int main(){
void maiorMenor(int *vet, int tam, int *menor, int *maior){
    int i;
    *menor = *vet;
    *maior = *vet;
    for(i = 1; i < tam; i++){
        if(*menor > *(vet + i))
            *menor = *(vet + i);
        if(*maior < *(vet + i))
            *maior = *(vet + i);
    }
}

int main(){
    int menor, maior, v[10] = {45,89,69,23,14,75,2,45,100,58};

    printf("Menor: %d\tMaior: %d\n", menor, maior);
    maiorMenor(v, 10, &menor, &maior);
    printf("Menor: %d\tMaior: %d\n", menor, maior);

    return 0;
 }
}

73° RESPOSTA
#include <stdio.h>
#include <conio.h>

int main(){
    
    int a=0,i,j,w,flag;
    int vetor[10],iguais[10];
    
    for(i=0;i<10;i++){
        printf("Entre com o elemento[ %d ] : ",i+1);
        scanf("%d",&vetor[i]);
    }
    for(i=0; i<10; i++){
        for(j=0; j<10; j++){
            flag=0;
            if(vetor[i]==vetor[j] && i != j){
                for(w=0; w<10; w++){
                    if(iguais[w] == vetor[j])
                        flag=1;
                }
                if(flag==0){
                    iguais[a]=vetor[i];
                    a++;
                }
                
            }
        }
     }
     for(i=0; i<a; i++){
        printf("%d ",iguais[i]);
     }
     getch();
     return 0;
}

74° RESPOSTA
#include <stdio.h>
#include <stdbool.h>
#define TAM  20

int main() {

    int vet[TAM], i,j;
    bool rept;  

    for (i=0; i<TAM; i++) {
        printf("Digite o %do valor: ", i+1);
        scanf("%d", &vet[i]);
    }

    for (i=0; i<TAM; i++) {
        rept = false;
        for (j = 0; j < i; j++) {
            if (vet[i] == vet[j]) {
                rept = true; 
                break;
            }
        }
        if (!rept) { 
            printf("%d ", vet[i]);
        }
    }

    return 0;
}

76°RESPOSTA
#include <stdio.h>

int main(){
  int array[10];
      for (int i=0;i<40;i++){
          printf("ADD[%d]:: ",i+1); scanf("%d",&array[i]);
      }

      for (int a=0;a<40;a++){
          if (array[a]<0){
              array[0]=0;
          }
      }
  for (int q=0;q<40;q++){
      printf("%d\n",array[q]);
  }
 retorn 0;
