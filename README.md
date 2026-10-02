# 🧠 Cérebro de Reservatório de Mosca (Drosophila Connectomics)

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![NeuPrint](https://img.shields.io/badge/NeuPrint-Data-lightgrey.svg)](https://neuprint.janelia.org/)

## 📌 Visão Geral
Este projeto é uma simulação computacional avançada que explora a intersecção entre neurobiologia estrutural e arquiteturas de Inteligência Artificial. Utilizando dados reais do connectoma da mosca *Drosophila* extraídos via NeuPrint, o projeto modela a dinâmica de **Reservoir Computing** e simula a propagação de estímulos (Leaky Integrate-and-Fire) em uma rede neural biológica.

O objetivo principal é compreender como a topologia natural de uma rede influencia sua capacidade de reter memória e processar informações dinâmicas — conceitos fundamentais para a arquitetura de modelos de IA e, consequentemente, para a exploração de suas vulnerabilidades (AI Red Teaming).

## 🛠️ Tecnologias e Ferramentas
*   **Linguagem:** Python
*   **Ambiente:** Jupyter Notebook / Google Colab
*   **Manipulação de Dados e Grafos:** NetworkX, Pandas, NumPy
*   **Visualização:** Matplotlib, Seaborn
*   **Extração:** API `neuprint-python`

## 🔬 Destaques Técnicos e Complexidade
Apesar de ser um projeto de pesquisa independente desenvolvido no início da graduação em Engenharia de Software, este repositório aborda problemas complexos de computação científica:

*   **Extração e Mapeamento de Grafos Densos:** Consulta à base de dados do Janelia Research Campus para mapear o neurônio `12811` e seus 730 parceiros sinápticos, gerando uma matriz de adjacência de 731x731.
*   **Análise Topológica:** Cálculo de métricas de rede que comprovam a eficiência biológica, identificando uma taxa de reciprocidade de ~42,8% e a predominância de ciclos curtos (triângulos).
*   **Simulação de Spikes (LIF):** Implementação de um Painel Dinâmico de Spikes baseado no modelo *Leaky Integrate-and-Fire*, simulando como a rede propaga e dissipa sinais ao longo do tempo.
*   **Métricas de Reservoir Computing:** Comparação de desempenho de memória (curva $R^2$) entre o connectoma biológico estruturado e redes de controle aleatórias.
*   **Otimização de Hardware:** Estruturação do código para execução eficiente em ambientes de nuvem (Google Colab), contornando limitações de hardware local para o processamento de álgebra linear e autovalores complexos.

## 🎯 Por que isso importa? (Perspectiva de AI Security)
Compreender a mecânica de como uma rede processa estímulos, retém contexto (memória de reservatório) e reage a inputs estruturados é o primeiro passo para realizar engenharia reversa do "comportamento" de modelos de linguagem (LLMs). 

Este estudo anatômico serve como base técnica para atuar em **Cibersegurança e AI Red Teaming**, fornecendo a profundidade necessária para entender ataques como *Prompt Injection* e engenharia social direcionada a IAs a partir da raiz: a estrutura da rede.

## 📊 Análise Visual (Resultados da Simulação)

**Dinâmica Leaky Integrate-and-Fire (LIF)**
![Painel Dinâmico de Spikes](lif_dynamics_panel.png)

**Curva de Capacidade de Memória**
![Capacidade de Memória](memory_capacity_curve.png)


## 🚀 Como Executar
1. Clone este repositório:
   ```bash
   git clone [https://github.com/wellingtonsjbdev/projeto-drosophiala.git](https://github.com/wellingtonsjbdev/projeto-drosophiala.git)
