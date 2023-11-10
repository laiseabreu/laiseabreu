//Construa uma estrutura aluno com nome, número da matrícula e curso. 
//Leia do usuário a informação de 5 alunos, armazene em vetor dessa estrutura e 
//imprima os dados na tela.

#include <stdio.h>
#include <string.h>
#include <stdlib.h>

    struct CADASTRO{
    char nome[50];
    int matricula;
    char curso[50];
};   

int main()
{
    struct CADASTRO c[5];
    int i;
    for (i=0; i < 5; i++){
        printf("\nCADASTRO %d\n" ,i+1);
        printf("\n Nome do aluno:");
        scanf("%s",c[i].nome);
        printf("\n Numero da matricula:");
        scanf("%d",&c[i].matricula);
        printf("\n Curso:");
        scanf("%s",c[i].curso);
    }
    for (i=0; i < 5; i++){
        printf("\nCADASTRO %d\n",i+1);
        printf("\n Nome = %s",c[i].nome);
        printf("\n Matricula = %d",c[i].matricula);
        printf("\n Curso = %s\n",c[i].curso);
    }

    return 0;
}

