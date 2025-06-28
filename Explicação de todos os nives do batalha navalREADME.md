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

# Nível Aventureiro:

Melhorias e explicações:
Enumeração de orientações:

Adicionei um tipo Orientacao para representar os diferentes tipos de posicionamento (horizontal, vertical, diagonal principal e diagonal secundária).

Validação de posições diagonais:

A função posicaoValida foi expandida para verificar:
Diagonal principal: onde linha e coluna aumentam juntas (i == j)
Diagonal secundária: onde linha aumenta enquanto coluna diminui (i + j == TAMANHO - 1)

Posicionamento de navios diagonais:
A função posicionarNavio agora trata os quatro tipos de orientação.

O programa posiciona:

1 navio horizontal
1 navio vertical
1 navio na diagonal principal
1 navio na diagonal secundária

Saída esperada:

text
Navio horizontal posicionado com sucesso na linha 2, coluna 3.
Navio vertical posicionado com sucesso na linha 5, coluna 7.
Navio diagonal principal posicionado com sucesso na linha 1, coluna 1.
Navio diagonal secundaria posicionado com sucesso na linha 2, coluna 7.

Tabuleiro de Batalha Naval:
    0  1  2  3  4  5  6  7  8  9 
 0  0  0  0  0  0  0  0  0  0  0 
 1  0  3  0  0  0  0  0  0  0  0 
 2  0  0  0  3  3  3  0  3  0  0 
 3  0  0  0  0  0  0  0  0  3  0 
 4  0  0  0  0  0  0  0  0  0  0 
 5  0  0  0  0  0  0  0  3  0  0 
 6  0  0  0  0  0  0  0  3  0  0 
 7  0  0  0  0  0  0  0  3  0  0 
 8  0  0  0  0  0  0  0  0  0  0 
 9  0  0  0  0  0  0  0  0  0  0 

Legenda:
0 - Agua
3 - Navio
O programa agora suporta todos os tipos de posicionamento necessários e valida corretamente as posições dos navios, incluindo os casos diagonais.

# Nível Mestre:

Matrizes de Habilidade:
Adicionei três tipos de habilidades (Cone, Cruz e Octaedro)
Cada habilidade é representada por uma matriz 5x5
A função criarHabilidade gera os padrões específicos para cada tipo

Padrões das Habilidades:
Cone: Forma triangular que se expande para baixo
Cruz: Linha horizontal e vertical que se cruzam no centro
Octaedro: Forma de losango (diagonais que se expandem do centro)

Aplicação das Habilidades:
A função aplicarHabilidade sobrepõe a matriz de habilidade no tabuleiro
As áreas afetadas são marcadas com o valor 5
As habilidades respeitam os limites do tabuleiro

Visualização:

O tabuleiro mostra claramente:
Água (0)
Navios (3)
Áreas de habilidade (5)

Saída esperada:

text
Tabuleiro de Batalha Naval com Habilidades:
    0  1  2  3  4  5  6  7  8  9 
 0  0  0  0  0  0  0  0  0  0  0 
 1  0  3  0  0  0  0  0  0  0  0 
 2  0  0  0  3  3  3  0  3  0  0 
 3  0  0  0  0  0  0  5  0  3  0 
 4  0  0  5  0  5  5  5  0  0  0 
 5  0  0  5  0  0  0  0  3  0  0 
 6  0  0  5  0  0  0  0  3  0  0 
 7  0  5  5  5  5  5  0  3  0  0 
 8  0  0  5  0  0  0  0  0  0  0 
 9  0  0  0  0  0  0  0  0  0  0 

Legenda:
0 - Agua
3 - Navio
5 - Area afetada por habilidade
O programa agora mostra claramente as áreas de efeito das três habilidades especiais sobrepostas ao tabuleiro de batalha naval, mantendo a visualização dos navios posicionados anteriormente.
