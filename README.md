# 📚 Pilhas (LIFO - Last In First Out)

Implementação de uma estrutura de dados de **Pilha** (Stack) em Java, seguindo o padrão LIFO (o último elemento inserido é o primeiro a ser removido).

---

## 📋 Descrição das Classes

### `No.java`
Representa um elemento individual da pilha.

**Campos:**
- `dado` (int) - valor armazenado no nó
- `refNo` - referência para o próximo nó na pilha

**Métodos:**
- `getters/setters` - acesso aos dados
- `toString()` - retorna a representação no formato `No{dado=...}`

---

### `Pilha.java`
Gerencia a estrutura de dados da pilha.

**Atributos:**
- `refNoEntradaPilha` - referência ao topo da pilha

**Métodos principais:**
- **`push(No novoNo)`** - insere um novo nó no topo e encadeia com o topo anterior
- **`pop()`** - remove e retorna o elemento do topo
- **`top()`** - retorna o elemento do topo sem remover
- **`isEmpty()`** - verifica se a pilha está vazia
- **`toString()`** - imprime todos os elementos da pilha (do topo para a base)

---

### `Main.java`
Classe principal que demonstra o funcionamento da pilha.

**Fluxo de execução:**
1. Cria uma nova pilha
2. Empilha nós com valores de 1 a 6
3. Imprime o estado da pilha
4. Remove o elemento do topo com `pop()` e exibe o resultado
5. Imprime a pilha após a remoção
6. Consulta o topo com `top()` e verifica se está vazia com `isEmpty()`

---

## ⚙️ Fluxo de Execução

```
Estado Inicial: Pilha vazia

Após push(1) até push(6):
Topo → 6 → 5 → 4 → 3 → 2 → 1 → (base)

Após pop():
- Elemento removido: 6
- Topo → 5 → 4 → 3 → 2 → 1 → (base)

top(): Retorna 5
isEmpty(): Retorna false
```

---

## 🚀 Como Usar

1. Clone ou baixe o repositório
2. Compile os arquivos Java
3. Execute a classe `Main`

```bash
javac *.java
java Main
```

---

## 📝 Características

✅ Implementação de Pilha com encadeamento dinâmico  
✅ Operações essenciais: push, pop, top, isEmpty  
✅ Representação em String formatada  
✅ Exemplo prático de uso na classe Main