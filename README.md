# softwareResultadoPartidaFutebolEmC
Seguindo no aprendizado da linguagem C, elaborei um software onde o usuário informa o número de gols das equipes e o programa emite uma mensagem informando o vencedor e o placar do jogo.

#include <stdio.h>
#include <locale.h>

int main()
{
    int placarTimeUm = 0;
    int placarTimeDois = 0;

    setlocale(LC_ALL,"Portuguese");    

    printf("SOFTWARE DE RESULTADO DE PARTIDA DE FUTEBOL! \n");
   
    printf("Digite o placar do primeiro time: \n");
    scanf("%d", &placarTimeUm);
   
    printf("Digite o placar do segundo time: \n");
    scanf("%d", &placarTimeDois);
   
    if (placarTimeUm > placarTimeDois) {
        printf("Time 1 venceu por: %d à %d!", placarTimeUm, placarTimeDois);
    }else if(placarTimeDois > placarTimeUm){
        printf("Time 2 venceu por: %d à %d!", placarTimeDois, placarTimeUm);
    }else {
        printf("A partida terminou empatada em: %d à %d!", placarTimeDois, placarTimeUm);
    };
   
    return 0;
};
