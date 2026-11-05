# Bolo da Lara

Projeto final da disciplina de Introdução a Algoritmos, desenvolvido em Python com a biblioteca Pygame.

## Integrantes do grupo

- Gabriela Gomes Mattoso
- Livia Hilbert de Oliveira
- Isabella Oliveira Araújo Barbosa Moreira
- Giovanna Brito Silva Ribeiro

## Sobre o jogo

Bolo da Lara é um jogo de cliques rápidos em que o jogador acompanha o personagem Lara durante o preparo de uma receita de bolo. A experiência é dividida em quatro etapas: selecionar os ingredientes, misturar a massa, assar e decorar. O jogador precisa seguir a sequência indicada e administrar o tempo para obter uma boa pontuação.

## Estrutura do repositório

- `main.py`: código principal do jogo. Contém a implementação da aplicação, das telas, das etapas e das interações realizadas pelo jogador.
- `testesdeverificacao`: arquivo com testes automatizados das regras e das funções relacionadas à pontuação, bônus por tempo, mensagens de resultado, etapas e armazenamento de recordes.
- `docs/proposta`: documento com a proposta inicial do jogo, incluindo ideia, objetivo, regras planejadas, elementos previstos, controles e testes considerados durante o planejamento.
- `recordes_bolo_lara.json`: arquivo criado automaticamente pelo jogo para armazenar os recordes. Ele é gerado durante a execução e não precisa ser enviado previamente ao repositório.

## Objetivo do jogador

Completar as quatro etapas da receita — ingredientes, misturar, assar e decorar — da forma mais eficiente possível, acumulando pontos e buscando alcançar cinco estrelas ao final.

## Regras do jogo

- Seguir a receita na ordem indicada.
- Concluir uma etapa antes de avançar para a próxima.
- Clicar em um ingrediente errado desconta 40 pontos.
- Cada etapa possui um cronômetro; esgotar o tempo desconta 50 pontos.
- Elementos ainda não desbloqueados não respondem à interação.
- Os erros reduzem a pontuação, mas não encerram imediatamente o jogo.
- Ao final, a pontuação é apresentada em estrelas (de zero a cinco), acompanhada de uma mensagem da Lara.

## Controles

O jogo utiliza o mouse:

- **Arrastar:** mover ingredientes e a massa para as áreas correspondentes, como o forno.
- **Girar o mouse dentro da tigela:** misturar a massa.
- **Clicar:** selecionar ingredientes e decorações, confirmar ações e navegar pelos menus.

## Como executar o projeto

É necessário ter Python instalado. Na pasta em que deseja salvar o projeto, execute:

```bash
git clone https://github.com/gabrielagmattoso/Jogo-Desenvolvido-em-Python---Bolo-do-Lara-.git
cd Jogo-Desenvolvido-em-Python---Bolo-do-Lara-
pip install pygame
python main.py
```

## Como executar os testes

Na pasta principal do repositório, execute:

```bash
python testesdeverificacao
```

O arquivo de testes apresenta no terminal quantos testes passaram e quantos falharam.

## Testes contemplados

- **Pontuação e estrelas:** verifica o cálculo das estrelas para diferentes pontuações.
- **Penalidades:** verifica o desconto por erro e impede que a pontuação fique negativa.
- **Mensagens de resultado:** verifica as mensagens exibidas para diferentes faixas de desempenho.
- **Bônus por tempo:** verifica o cálculo do bônus conforme o tempo restante.
- **Etapas do jogo:** verifica a quantidade e a ordem das quatro fases.
- **Recordes:** verifica o salvamento, a ordenação e o limite de dez registros.
