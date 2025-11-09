# Queue and Stack System  
Sistema em Java desenvolvido para **gerenciar e simular operações com Fila e Pilha** implementadas sobre **listas encadeadas autorais**, reforçando o domínio sobre estruturas dinâmicas, ponteiros e complexidade. Projeto acadêmico ideal para disciplinas de Estruturas de Dados, com foco em clareza, eficiência e autoria comprovada.  

<p align="center">
  <img src="https://img.shields.io/badge/Java-17%2B-blue" />
  <img src="https://img.shields.io/badge/Build-javac%2Fjar-informational" />
  <img src="https://img.shields.io/badge/License-MIT-success" />
</p>

---

## Objetivos do projeto  
* Demonstrar a implementação **manual de Fila e Pilha** utilizando **listas encadeadas**.  
* Compreender as diferenças operacionais entre as estruturas FIFO e LIFO.  
* Aplicar as operações clássicas de inserção, remoção e iteração em nós.  
* Garantir manipulação eficiente de dados e consistência nas operações.  

---

## Funcionalidades principais  
* Inserir elementos na **fila** (ordem FIFO).  
* Remover elementos da fila (desenfileirar).  
* Inserir elementos na **pilha** (ordem LIFO).  
* Remover elementos da pilha (desempilhar).  
* Exibir o conteúdo atual das estruturas.  
* Demonstrar os efeitos das operações em tempo real via terminal.  

---

## Estruturas implementadas  
**Lista Encadeada:** Base para as estruturas de Fila e Pilha. Possui classe `No<T>` com ponteiro para o próximo elemento. Permite inserção, remoção e busca sequencial. Complexidade média das operações: Inserção O(1), Remoção O(1) nas extremidades, Busca O(n).  

**Fila Encadeada:** Segue o princípio **First In, First Out (FIFO)**. Operações principais: `enfileirar(T elemento)` insere no final, `desenfileirar()` remove do início, `primeiro()` retorna o primeiro elemento, `vazia()` verifica se a fila está vazia.  

**Pilha Encadeada:** Segue o princípio **Last In, First Out (LIFO)**. Operações principais: `empilhar(T elemento)` insere no topo, `desempilhar()` remove o elemento do topo, `topo()` retorna o elemento do topo, `vazia()` verifica se a pilha está vazia.  

---


## Modelo de dados  
**Classe Elemento:** valor genérico (`T`), método `toString()` retorna representação textual.  
**Classe No:** dado (`T`) e ponteiro `proximo` para o próximo nó.  

---

## Operações e complexidade  
| Operação | Estrutura | Complexidade | Descrição |
|-----------|------------|--------------|------------|
| Inserção | Fila/Pilha | O(1) | Adiciona elemento ao final (fila) ou topo (pilha) |
| Remoção | Fila/Pilha | O(1) | Remove o primeiro (fila) ou topo (pilha) |
| Busca | Lista | O(n) | Percorre os nós encadeados |
| Impressão | Todas | O(n) | Exibe todos os elementos |

---

## Validações  
* Evita remoção em estrutura vazia.  
* Exibe mensagens claras para o usuário.  
* Garante integridade dos ponteiros após remoções.  

---

## Diagrama de funcionamento  
```mermaid
flowchart TD
  subgraph Estruturas
    N[No]
    L[ListaEncadeada]
    F[FilaEncadeada]
    P[PilhaEncadeada]
  end
  N --> L
  L --> F
  L --> P
