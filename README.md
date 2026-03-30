PROJETO APLICADO III
Sistema de Recomendação de Produtos Fitness

Este projeto tem como objetivo o desenvolvimento de um sistema de recomendação de produtos fitness, utilizando técnicas de ciência de dados e aprendizado de máquina aplicadas a dados reais de interações entre usuários e produtos da Amazon.

O trabalho foi desenvolvido no contexto da disciplina Projeto Aplicado III – Ciência de Dados, da Universidade Presbiteriana Mackenzie.

Autores

KARLA MARIA RAMOS DA SILVA (10730503) 
OSCAR LUZ (10435099)
RAFAEL HESSEL SICHETTI (10375395) 

Objetivo do Projeto

Desenvolver um sistema de recomendação capaz de sugerir produtos fitness relevantes aos usuários, com base em suas interações e avaliações registradas no dataset.

O sistema deverá:

Identificar padrões de comportamento de consumo
Sugerir produtos semelhantes ou de interesse
Apoiar a tomada de decisão dos consumidores
Dataset Utilizado

O projeto utiliza o dataset de avaliações de produtos da Amazon, disponibilizado pelo pesquisador Julian McAuley da University of California San Diego.

Categoria utilizada:

Sports & Outdoors (produtos fitness)

O dataset contém:

usuários (reviewerID)
produtos (asin)
avaliações (ratings)
textos e metadados
Etapas do Projeto

O projeto segue um pipeline estruturado de ciência de dados:

1. Pré-processamento dos dados
Limpeza dos dados
Remoção de valores nulos
Seleção das variáveis relevantes
2. Análise exploratória (EDA)
Distribuição das avaliações
Quantidade de usuários e produtos
Produtos mais avaliados
3. Vetorização / Estruturação
Construção da matriz usuário × produto
4. Modelagem
Implementação de sistema de recomendação utilizando:
Filtragem colaborativa
5. Avaliação
Análise das recomendações geradas
Validação qualitativa dos resultados
Estrutura do Projeto
├── recommender_system.py
├── notebook_recommendation.ipynb
├── data/
├── outputs/
├── requirements.txt
└── README.md
Tecnologias Utilizadas
Python 3.10+
pandas
numpy
scikit-learn
matplotlib
Como Executar o Projeto
1) Execução via Script
python recommender_system.py --data_path reviews.json --out_dir outputs

O script realiza:

Carregamento dos dados
Tratamento e limpeza
Construção da matriz usuário-produto
Geração de recomendações
Salvamento dos resultados
2) Execução via Notebook
jupyter notebook

Abrir:

notebook_recommendation.ipynb

O notebook contém:

Análise exploratória
Construção do modelo
Geração de recomendações
Visualizações
Resultados Esperados

O sistema será capaz de gerar recomendações como:

“Usuários que avaliaram este produto também avaliaram...”
“Produtos semelhantes com base no comportamento de outros usuários”

Exemplo:

Produto A → recomenda Produto B, C e D
