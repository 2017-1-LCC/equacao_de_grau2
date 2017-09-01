# equacao_de_grau2
Uma equação do segundo grau possui uma incógnita de expoente 2. 
O método de Bhaskara é uma opção para encontrar os resultados desse tipo de equação.

/**
* INSTITUTO FEDERAL DE EDUCAÇÃO, CIÊNCIA E TECNOLOGIA BAIANO
*               CAMPUS DE SENHOR DO BONFIM
*          LICENCIATURA EM CIÊNCIAS DA COMPUTAÇÃO
*
*
* Jefferson Medeiros da Silva
* 23/08/2017
*
*/

#include <stdio.h>
#include <math.h> //inclusao da biblioteca math.h para calculo da raiz quadrada

int main() //declaracao da funcao main

{
    int a,b,c,delta; //declacarao das variaveis inteiras
    float raiz,x1,x2; //declaracao das variaveis reais
    printf ("________________________________________________________________________________");
    printf ("\n  BBB     H   H     AAA      SSS      K   K       AAA      RRRR      AAA      ");
    printf ("\n  B   B   H   H    A   A    S         K  K       A   A     R    R   A   A     " );
    printf ("\n  BBB     HHHHH    A A A     SSS      KK         A A A     R R R    A A A     ");
    printf ("\n  B   B   H   H    A   A        S     K  K       A   A     R   R    A   A     ");
    printf ("\n  BBB     H   H    A   A     SSS      K   K      A   A     R    R   A   A     \n");
    printf ("________________________________________________________________________________\n");
    printf ("                      Desenvolvido por Jefferson Medeiros  \n\n");
    printf ("\n                         Digite o valor do fator A: ");
    scanf  ("%d", &a); //recebe um valor e o adiciona a variavel a
    printf ("________________________________________________________________________________");
    printf ("\n                         Digite o valor do fator B: ");
    scanf ("%d", &b);//recebe um valor e o adiciona a variavel b
    printf ("________________________________________________________________________________");
    printf ("\n                         Digite o valor do fator C: ");
    scanf ("%d", &c); //recebe um valor e o adiciona a variavel c
    printf ("________________________________________________________________________________");
    delta = (b*b)-4*a*c; //calculo do delta
    if ((delta < 0)) //verifica se o delta e menor que zero
    {
        printf ("\n     O delta e %d, ou seja, negativo, portanto nao existem raizes reais! \n\n", delta);
        printf ("________________________________________________________________________________");
        getchar();
    }
    else //caso o delta nao for menor que zero, executa o bloco de instrucoes abaixo
    {
        raiz = sqrt(delta); //atribui o valor da raiz quadrada de delta a variavel raiz
        x1 = (-b+raiz)/2*a; //a variavel x1, recebe o resultado da conta ao lado
        x2 = (-b-raiz)/2*a;//a variavel x2, recebe o resultado da conta ao lado
        printf ("\n                O resultado e: X1 = %.2f e X2 = %.2f !\n\n", x1,x2);
        printf ("_______________________________________________________________________________\n");
        getchar(); //espera que o usuario digite uma tecla para finalizar a execucao
    }
}
