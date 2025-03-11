# Atividade de Comparação de Algoritmos de Ordenação

## Objetivo
Os alunos deverão implementar e comparar a performance de diferentes algoritmos de ordenação, analisando a complexidade computacional e a quantidade de operações executadas. Para garantir uma comparação justa, os dados a serem ordenados devem ser gerados aleatoriamente e armazenados em um arquivo, que será lido e processado por cada algoritmo.

Além disso, os alunos devem utilizar o padrão de projeto Strategy para implementar os algoritmos de ordenação de forma modular e extensível. A coleta de evidências da execução deve ser registrada utilizando OpenTelemetry, e os logs devem ser visualizados por meio de uma ferramenta open-source apropriada.

## Requisitos da Atividade

### Gerador de Dados
- Criar um programa que gere um conjunto de números aleatórios e os salve em um arquivo de texto ou binário.
- O tamanho do conjunto de dados deve ser parametrizável (ex: 1.000, 10.000, 100.000 números).

### Implementação dos Algoritmos de Ordenação
- Implementar os seguintes algoritmos de ordenação:
- **Básicos:**
 - Bubble Sort
 - Bubble Sort Melhorado
 - Insertion Sort
 - Selection Sort
- **Avançados (Dividir para Conquistar):**
 - Quick Sort
 - Merge Sort
 - Tim Sort
- **Outros Algoritmos Sugeridos:**
  - Heap Sort
  - Counting Sort (para números inteiros limitados)
  - Radix Sort (para inteiros)
  - Shell Sort
  
- Utilizar **padrão Strategy** para a implementação modular dos algoritmos.

  ## Execução e Comparação
  - Cada algoritmo deve ser executado carregando os mesmos dados do arquivo gerado.
  - Coletar métricas de desempenho, incluindo:
     - Tempo de execução (milissegundos)
     - Quantidade de comparações
     - Quantidade de trocas/movimentações
  - Cada execução deve ser repetida várias vezes para garantir uma média confiável.
 
  ## Registro de Logs com OpenTelemetry
  - Registrar logs para cada execução, incluindo:
     - Nome do algoritmo
     - Tamanho do conjunto de dados
     - Tempo de execução, etapas e passos, ...
     - Número de operações realizadas (comparações e trocas)
  - Utilizar uma ferramenta open-source para visualização dos logs, como:
     - **Jaeger** (tracing de execução)
     - **Prometheus** + **Grafana** (monitoramento de métricas)
     - **Elasticsearch** + **Kibana** (análise de logs)
   
 ## Entrega e Relatório
 Cada equipe deve entregar um relatório técnico contendo:
 1. Código-fonte documentado e organizado.
 2. Explicação do uso do padrão Strategy.
 3. Descrição do processo de geração dos dados.
 4. Métricas e gráficos comparativos de desempenho.
 5. Descrição da ferramenta utilizada para logs e análise dos resultados.
 6. Conclusão: qual algoritmo apresentou melhor desempenho em diferentes cenários? Por que apresentou? Vale a pena usar Dividir e Conquistar?

A submissão pode ser feita via repositório GitHub/GitLab, link no relatório técnico entregue da da submissão.

## Critérios de Avaliação
| **Critério**  | **Pontuação** |
| ------------- | ------------- |
| Implementação correta dos algoritmos  |	20% |
| Uso adequado do padrão Strategy  | 	10% |
| Geração e leitura correta dos dados | 	10% |
| Registro e análise de logs com OpenTelemetry | 	10% |
| Relatório técnico bem estruturado |	10% | 

**Total**: 50% da N1.

## Recomendações
- Dividir as tarefas entre os integrantes da equipe para otimizar o tempo.
- Testar com diferentes tamanhos de entrada para obter comparações robustas.
- Verificar a documentação das ferramentas de monitoramento antes de implementar.

**Divirtam-se!**
