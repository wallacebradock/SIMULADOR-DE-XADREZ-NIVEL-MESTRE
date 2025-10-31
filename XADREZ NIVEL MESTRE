#include <stdio.h>

int main() {
    printf("SIMULADOR DE XADREZ NIVEL MESTRE\n\n");
    
    // =============================================
    // MOVIMENTO DA TORRE
    // =============================================
    printf("1 - MOVIMENTO DA TORRE\n");
    printf("==========================\n");
    
    int casas_torre_direita = 3;
    int casas_torre_cima = 2;
    
    // Torre movendo para a direita
    printf("Torre movendo %d casas para a direita:\n", casas_torre_direita);
    for (int i = 1; i <= casas_torre_direita; i++) {
        printf("  Passo %d: Direita\n", i);
    }
    
    // Torre movendo para cima
    printf("\nTorre movendo %d casas para cima:\n", casas_torre_cima);
    for (int i = 1; i <= casas_torre_cima; i++) {
        printf("  Passo %d: Cima\n", i);
    }
    
    // =============================================
    // MOVIMENTO DO BISPO
    // =============================================
    printf("\n2 - MOVIMENTO DO BISPO\n");
    printf("============================\n");
    
    int movimentos_bispo = 3;
    int contador_diagonal = 0;
    
    printf("Bispo movendo %d vezes na diagonal (Cima + Direita):\n", movimentos_bispo);
    
    // Loop while para controlar o número de movimentos diagonais
    while (contador_diagonal < movimentos_bispo) {
        printf("  Movimento diagonal %d:\n", contador_diagonal + 1);
        
        // Loop for para decompor o movimento diagonal
        for (int passo = 1; passo <= 2; passo++) {
            if (passo == 1) {
                printf("    - Cima\n");
            } else {
                printf("    - Direita\n");
        }
        }
        contador_diagonal++;
    }
    
    // =============================================
    // MOVIMENTO DO CAVALO - MOVIMENTO EM "L"
    // =============================================
    printf("\n3 - MOVIMENTO DO CAVALO\n");
    printf("=============================\n");
    
    /*
    LÓGICA AVANÇADA DO MOVIMENTO DO CAVALO:
    O Cavalo possui 8 movimentos possíveis em L, mas neste simulador
    vamos demonstrar o movimento: 2 casas para BAIXO + 1 casa para ESQUERDA
    
    Estratégia com loops aninhados:
    - Loop externo (for): Controla as duas fases do movimento L
    - Loop interno (while): Controla a repetição de cada direção
    */
    
    const int FASE_VERTICAL = 2;    // 2 casas para baixo
    const int FASE_HORIZONTAL = 1;  // 1 casa para esquerda
    
    printf("Cavalo executando movimento em L:\n");
    printf("(2 casas Baixo + 1 casa Esquerda)\n\n");
    
    // LOOP EXTERNO: Controla as duas fases do movimento em L
    for (int fase_movimento = 0; fase_movimento < 2; fase_movimento++) {
        
        if (fase_movimento == 0) {
            // FASE 1: Movimento Vertical (2 casas para baixo)
            printf("Fase 1 - Movimento Vertical:\n");
            int contador_vertical = 0;
            
            // LOOP INTERNO: Executa os 2 movimentos para baixo
            while (contador_vertical < FASE_VERTICAL) {
                printf("  Casa %d: Baixo\n", contador_vertical + 1);
                contador_vertical++;
            }
            
        } else {
            // FASE 2: Movimento Horizontal (1 casa para esquerda)
            printf("Fase 2 - Movimento Horizontal:\n");
            int contador_horizontal = 0;
            
            // LOOP INTERNO: Executa o movimento para esquerda
            while (contador_horizontal < FASE_HORIZONTAL) {
                printf("  Casa %d: Esquerda\n", contador_horizontal + 1);
                contador_horizontal++;
            }
        }
    }
    
    // =============================================
    // RESUMO DOS MOVIMENTOS
    // =============================================
    printf("\n4 - RESUMO DO SIMULADOR\n");
    printf("=============================\n");
    printf("Peças simuladas:\n");
    printf("- Torre: Movimento reto (horizontal/vertical)\n");
    printf("- Bispo: Movimento diagonal\n");
    printf("- Cavalo: Movimento em L (2+1 casas)\n");
    printf("\nTotal de direcoes impressas:\n");
    
    // Cálculo demonstrativo do total de direções
    int total_direcoes = 0;
    
    // Torre: direita + cima
    total_direcoes += casas_torre_direita + casas_torre_cima;
    
    // Bispo: 2 direções por movimento diagonal
    total_direcoes += movimentos_bispo * 2;
    
    // Cavalo: baixo + esquerda
    total_direcoes += FASE_VERTICAL + FASE_HORIZONTAL;
    
    printf("Torre: %d direcoes\n", casas_torre_direita + casas_torre_cima);
    printf("Bispo: %d direcoes\n", movimentos_bispo * 2);
    printf("Cavalo: %d direcoes\n", FASE_VERTICAL + FASE_HORIZONTAL);
    printf("TOTAL: %d direcoes impressas\n", total_direcoes);
    
    printf("\nSIMULACAO CONCLUIDA\n");
    
    return 0;
}
