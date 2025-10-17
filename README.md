# Sistema de Gerenciamento de Atendimento ao Cliente

Trabalho prático da disciplina de Resolução de Problemas Estruturados.  
Objetivo: implementar uma **Pilha** e uma **Fila** utilizando **lista encadeada**, sem usar arrays ou bibliotecas prontas, para simular um sistema de atendimento.

## Estruturas Implementadas

### Pilha (Histórico de Solicitações)
- Cada nó guarda **id**, **descrição**, **data e hora** da solicitação.
- Operações:
  - `push`: adiciona nova solicitação no topo.
  - `pop`: remove a solicitação mais recente.
  - `peek`: consulta a última sem remover.
  - `isEmpty`: verifica se a pilha está vazia.
  - `imprimir`: mostra histórico do topo para a base.

### Fila (Ordem de Atendimento)
- Cada nó guarda **id**, **nome** e **motivo** do cliente.
- Operações:
  - `enqueue`: adiciona cliente ao final da fila.
  - `dequeue`: remove o cliente da frente (atendido).
  - `peek`: consulta o próximo sem remover.
  - `isEmpty`: verifica se a fila está vazia.
  - `imprimir`: mostra a fila da frente para trás.

## Regras Seguidas

- **Sem uso de arrays ou coleções** (`ArrayList`, `LinkedList`, etc.).
- **Sem TADs prontos**.
- **Apenas String, int, float, try-catch, throws e entrada simples**.
- `length` usado somente em `String` (não necessário neste caso).
- Nenhuma função automatizada ou inteligência artificial utilizada no desenvolvimento.

## Como Compilar e Executar

No terminal:

```bash
cd src
javac Main.java
java Main
