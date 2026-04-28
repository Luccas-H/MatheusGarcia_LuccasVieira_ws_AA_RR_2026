# Análise Experimental e Profunda: Selection Sort 🚀

Este repositório apresenta um estudo técnico detalhado sobre o comportamento do algoritmo **Selection Sort**. O diferencial deste projeto é a análise de desempenho baseada em **datasets externos (arquivos)**, permitindo uma investigação profunda sobre como a implementação lida com diferentes volumes e distribuições de dados.

O projeto foi desenvolvido como parte das atividades de **Análise de Algoritmos** na Universidade Federal de Roraima (UFRR).

## 📋 Sumário
- [Visão Geral](#-visão-geral)
- [O Algoritmo](#-o-algoritmo)
- [Metodologia e Arquivos](#-metodologia-e-arquivos)
- [Análise de Complexidade](#-análise-de-complexidade)

---

## 🔍 Visão Geral
Diferente de testes meramente sintéticos, este projeto foca na **análise profunda**. Isso inclui a revisão da eficiência do código C implementado, o impacto da leitura de arquivos de entrada no tempo total de execução e a visualização detalhada da curva de crescimento do algoritmo em comparação com limites teóricos.

## 💡 O Algoritmo: Selection Sort
A implementação foca na ordenação por comparação que, a cada iteração, busca o menor elemento e o posiciona no início do array.
* **Foco do estudo:** Observar o custo fixo de trocas vs. o custo crescente de comparações.
* **Implementação:** O código foi otimizado para clareza acadêmica, facilitando a análise da estrutura de loops aninhados.

---

## 🧪 Metodologia e Arquivos
O projeto utiliza arquivos de texto para garantir a consistência dos testes:
1.  **Datasets:** Arquivos contendo ranges diversificados de números (ordenados, inversamente ordenados e aleatórios).
2.  **Entrada/Saída:** O script lê os dados dos arquivos, executa a ordenação e armazena os logs de tempo.
3.  **Análise de Código:** Revisão linha a linha para identificar gargalos operacionais.

---

## 📊 Análise de Complexidade

| Caso | Complexidade de Tempo | Complexidade de Espaço |
| :--- | :--- | :--- |
| **Melhor Caso** | $O(n^2)$ | $O(1)$ |
| **Caso Médio** | $O(n^2)$ | $O(1)$ |
| **Pior Caso** | $O(n^2)$ | $O(1)$ |

*Nota: Mesmo que o vetor esteja ordenado, o Selection Sort mantém sua complexidade quadrática devido à necessidade de percorrer o restante do array para confirmar o menor elemento.*

---

## ⚖️ Análise Comparativa: Selection vs. Quick Sort Otimizado

Para validar a eficiência da implementação, este estudo realizou um benchmark comparativo com um **Quick Sort Otimizado**. 

Enquanto o Selection Sort serviu como base para análise de algoritmos quadráticos, o Quick Sort foi utilizado para demonstrar a performance de algoritmos de divisão e conquista em cenários reais.

### Diferenciais da Otimização do Quick Sort:
* **Escolha do Pivô:** Implementação de estratégias para evitar o pior caso ($O(n^2)$), como o uso de pivô aleatório ou mediana de três.
* **Recursividade:** Controle de profundidade de recursão para garantir estabilidade em ranges extremamente altos de dados.
* **Performance:** Demonstração prática da barreira de desempenho entre as complexidades $O(n^2)$ e $O(n \log n)$.

| Métrica | Selection Sort | Quick Sort Otimizado |
| :--- | :--- | :--- |
| **Escalabilidade** | Baixa (sofre com ranges altos) | Alta (estável em grandes volumes) |
| **Impacto de Arquivo** | Significativo no processamento | Mínimo perto da eficiência do código |
| **Comportamento** | Curva Quadrática | Curva Linear-Logarítmica |

---

## 🛠️ Configuração e Execução

### Pré-requisitos
* Python 3.x
* Matplotlib (para visualização dos resultados)
* GCC

### Instalação e Uso
1. Clone o repositório:
   ```bash
   git clone [https://github.com/Mtheusgs/MatheusGarcia_LuccasVieira_ws_AA_RR_2026.git](https://github.com/Mtheusgs/MatheusGarcia_LuccasVieira_ws_AA_RR_2026.git)
