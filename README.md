# LMSys Chatbot Arena

## Objetivo
Este projeto tem como objetivo propor, documentar e defender uma solução que determine qual resposta é melhor, ou se há um empate, com base em critérios definidos. A solução explora técnicas de aprendizado de máquina para análise de respostas em um ambiente de chatbot.

## Descrição

### Proposta
A abordagem principal utilizada é o Boosting, uma técnica de aprendizado de máquina que combina os resultados de vários modelos fracos para criar um modelo forte. Este processo utiliza uma sequência de interações, onde pesos são aplicados aos erros obtidos em cada treinamento.

**Exemplo**
O XGBoost é um algoritmo baseado em gradient boosting que utiliza árvores de decisão, onde cada árvore tenta corrigir os erros da anterior.

### Funcionalidades
Para a resolução deste problema, são extraídas características dos textos do dataset, incluindo:

- Tamanho dos textos;
- Palavras presentes na pergunta e nas respostas;
- Diferença entre as respostas, entre outras.

### Estrutura do Projeto
1 - Pré-processamento: Limpeza e preparação dos dados textuais.  
2 - Exploração de Dados: Análise exploratória para definir as features mais relevantes.  
3 - Modelagem: Aplicação e ajuste de modelos de classificação, como Gradient Boosting, XGBoost e CatBoost.

## Como Executar

```bash
# Clone este repositório:
git clone <URL_DO_REPOSITORIO>
cd nome-do-repositorio

# Instale as dependências necessárias:
pip install -r requirements.txt

# Execute o notebook:
# Abra o notebook 'lmsys-modelsboost.ipynb' em seu ambiente Jupyter Notebook ou Google Colab
# e siga as instruções e células para realizar o treinamento e avaliação dos modelos.
