O que cada classe faz
No.java:
Representa um elemento da pilha.
Campos: dado (int) e refNo (referência para o próximo nó).
Tem getters/setters e toString() no formato No{dado=...}.
Pilha.java:
Guarda o topo em refNoEntradaPilha.
push(No novoNo): coloca um novo nó no topo e encadeia com o topo antigo.
pop(): remove e retorna o topo (com um detalhe de lógica atual, explicado abaixo).
top(): retorna o topo sem remover.
isEmpty(): verifica se a pilha está vazia.
toString(): imprime da cabeça para baixo (topo -> base).
Main.java:
Cria a pilha.
Empilha nós de 1 a 6.
Imprime a pilha.
Chama pop(), imprime o retorno e imprime a pilha novamente.
Chama top() e isEmpty() para demonstrar o comportamento.
Fluxo de execução atual
Após os push, o topo é 6.
O programa tenta remover com pop().
Depois consulta topo e vazio para mostrar estado da estrutura.
