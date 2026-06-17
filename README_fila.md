# Fila de Requisições

Sistema de fila de atendimento em C, implementado com fila encadeada (FIFO).
Cada requisição guarda nome, código de inscrição e código do procedimento.

## Estrutura dos arquivos

| Arquivo | Descrição |
|---|---|
| `main.c` | Programa principal, exemplo de uso da fila |
| `estrutura.h` / `estrutura.c` | Fila encadeada (criar, enfileirar, desenfileirar, tamanho, liberar) |
| `requisicao.h` / `requisicao.c` | Struct da requisição e função para criá-la |

## Como compilar

```bash
gcc main.c estrutura.c requisicao.c -o programa
```

## Como rodar

```bash
./programa
```

No Windows:

```bash
programa.exe
```

## O que o programa faz

1. Cria a fila.
2. Adiciona 3 requisições (João, Maria, Carlos).
3. Mostra o tamanho da fila.
4. Atende (desenfileira) o primeiro da fila.
5. Mostra o tamanho de novo.
6. Libera a memória.

## Saída esperada

```
Tamanho da fila: 3
Atendido: Joao (1)
Tamanho da fila: 2
```
