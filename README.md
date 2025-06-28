# Trabalho-da-faculdade-Wyden-FBV-Batalha-naval

Nível iniciante:

Definições iniciais:
Foram definidas constantes para o tamanho do tabuleiro (10x10), tamanho dos navios (3) e valores para água (0) e navio (3).

Funções principais:

inicializarTabuleiro(): Preenche toda a matriz com 0 (água).
posicaoValida(): Verifica se um navio pode ser posicionado nas coordenadas dadas, checando:
Se está dentro dos limites do tabuleiro
Se não há sobreposição com outros navios
posicionarNavio(): Coloca o valor 3 nas posições do tabuleiro ocupadas pelo navio.
exibirTabuleiro(): Mostra o tabuleiro formatado com números de linha/coluna e legenda.

Fluxo principal:

Inicializa o tabuleiro
Define as coordenadas dos navios (no código)
Tenta posicionar cada navio, verificando a validade da posição
Exibe o tabuleiro resultante

Saída esperada:
text
Navio horizontal posicionado com sucesso na linha 2, coluna 3.
Navio vertical posicionado com sucesso na linha 5, coluna 7.

Tabuleiro de Batalha Naval:
    0  1  2  3  4  5  6  7  8  9 
 0  0  0  0  0  0  0  0  0  0  0 
 1  0  0  0  0  0  0  0  0  0  0 
 2  0  0  0  3  3  3  0  0  0  0 
 3  0  0  0  0  0  0  0  0  0  0 
 4  0  0  0  0  0  0  0  0  0  0 
 5  0  0  0  0  0  0  0  3  0  0 
 6  0  0  0  0  0  0  0  3  0  0 
 7  0  0  0  0  0  0  0  3  0  0 
 8  0  0  0  0  0  0  0  0  0  0 
 9  0  0  0  0  0  0  0  0  0  0 

Legenda:
0 - Agua
3 - Navio
O programa posiciona corretamente os dois navios (um horizontal e outro vertical) sem sobreposição e dentro dos limites do tabuleiro.
