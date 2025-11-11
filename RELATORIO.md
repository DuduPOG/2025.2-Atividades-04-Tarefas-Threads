# Relatório de Observações - Atividade de Threads

## Informações do Aluno

- **Nome:** Eduardo Medeiros de Sousa Aguiar
- **Matrícula:** 20242014040005
- **Data:** 10/11/2025

## Ambiente de Execução

- [ ] Executado localmente
- [X] Executado em Docker/Fedora

**Sistema Operacional:** Windows 11 25H2  
**Processador:** AMD Ryzen 7 5700G  
**Número de Cores:** 8 cores, 16 threads

---

## Execução 1

### Resultados Observados

**Thread CPU (Thread 1):**

- Tempo de execução: 0.20 segundos
- Soma dos primos: 37550402023
- Ordem de conclusão: 3º (1ª, 2ª ou 3ª)

**Thread I/O (Thread 2):**

- Tempo de execução: 0 segundos
- Linhas processadas: 10000
- Ordem de conclusão: 1º (1ª, 2ª ou 3ª)

**Thread Mista (Thread 3):**

- Tempo de execução: 0.01 segundos
- Total de cálculos: 3482527859448382464
- Ordem de conclusão: 2º (1ª, 2ª ou 3ª)

**Tempo Total do Programa:** 0 segundos

### Observações sobre a Saída

Descreva como as mensagens das threads apareceram no console:

As mensagens foram mescladas, sendo executadas ao mesmo tempo e no final cada uma foi finalizada no seu tempo

---

## Execução 2 (Repetir para comparação)

### Resultados Observados:

**Thread CPU (Thread 1):**

- Tempo de execução: 0.20 segundos
- Ordem de conclusão: 3º (1ª, 2ª ou 3ª)

**Thread I/O (Thread 2):**

- Tempo de execução: 0.01 segundos
- Ordem de conclusão: 1º (1ª, 2ª ou 3ª)

**Thread Mista (Thread 3):**

- Tempo de execução: 0.01 segundos
- Ordem de conclusão: 2º (1ª, 2ª ou 3ª)

**Tempo Total do Programa:** 0 segundos

### Diferenças entre Execuções

Dessa vez o tempo de execução da Thread 2 pôde ser computado

---

## Análise e Conclusões

### 1. Qual thread terminou primeiro? Por quê?

I/O, pela menor demanda de processamento

### 2. Por que os tempos de execução variam entre diferentes execuções?

A carga do sistema pode aumentar por processos em segundo plano executados na máquina ou inconsistências no funcionamento do computador

### 3. Como o sistema operacional gerencia a execução das threads?

No Windows, por prioridade

### 4. Qual seria o impacto de aumentar o número de threads?

Otimizar os processos com processamento paralelo

### 5. O que aconteceria se executássemos as mesmas operações sequencialmente?

Poderia levar mais tempo pela demanda de processamento.

---

## Experimentos Adicionais (Opcional)

### Modificação 1: Aumentar NUM_ITERACOES

**Alteração realizada:** Mudei NUM_ITERACOES de 1000000 para 10000000

**Resultado observado:**

- Tempo da Thread CPU: 4.71 segundos
- Impacto no tempo total: Grande

**Conclusão:** _[O que você aprendeu com essa modificação?]_

### Modificação 2: Adicionar mais threads

**Alteração realizada:** Criei 3 threads CPU adicionais

**Resultado observado:** Aumento no tempo de execução

- Comportamento: A necessidade de processamento intensivo provocou uma perda de desempenho por causa da demanda pelas threads
- Impacto na performance: Médio

**Conclusão:** Em CPU-Bound, poucas threads não são eficientes para otimizar a execução de tarefas significativamente

---

## Conceitos Aprendidos

Liste os principais conceitos de sistemas operacionais que você compreendeu melhor com esta atividade:

1. Concorrência e paralelismo
2. Diferença entre operações CPU-bound e I/O-bound
3. Context Switching

---

## Dificuldades Encontradas

Descreva quaisquer problemas que enfrentou durante a atividade e como os resolveu:

Executar o programa no ambiente local, resolvi mudando o do prompt do powershell para o git bash

---

## Comentários Finais

_[Espaço para observações adicionais, sugestões ou comentários sobre a atividade]_

---

**Data de Conclusão:** 10/11/2025

**Assinatura:** Eduardo Medeiros
