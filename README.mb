# Análise de Segmentação de Clientes usando K-means

## 📊 Sobre o Projeto
Este projeto utiliza técnicas de machine learning, especificamente o algoritmo K-means, para realizar uma segmentação de clientes de um shopping center. O objetivo é identificar padrões de comportamento e criar estratégias de marketing personalizadas para diferentes grupos de clientes.

## 📋 Dataset
O dataset utilizado contém informações de 200 clientes com os seguintes atributos:
- CustomerID: Identificador único do cliente
- Gender: Gênero do cliente
- Age: Idade do cliente
- Annual Income (k$): Renda anual em milhares de dólares
- Spending Score (1-100): Score de gastos atribuído pelo shopping

## 🛠 Fases do Desenvolvimento

### 1. Exploração e Análise de Dados

#### Análise Exploratória Inicial
![Análise Exploratória](/images/exploratory_analysis.png)

A análise exploratória revelou:
- **Distribuição de Gênero**: Ligeira maioria de clientes femininas
- **Distribuição de Idade**: Concentração entre 25-35 anos
- **Renda Anual**: Maioria entre 40k-80k
- **Padrão de Gastos**: Distribuição trimodal (baixo, médio e alto consumo)

#### Correlações e Padrões
![Correlações](/images/correlation_matrix.png)

Principais insights das correlações:
- Correlação negativa entre Idade e Score de Gastos (-0.33)
- Correlação quase nula entre Renda e Gastos (0.009)
- Padrões distintos de comportamento por faixa etária

### 2. Pré-processamento dos Dados
- Tratamento de variáveis categóricas (Gender) usando one-hot encoding
- Padronização das variáveis numéricas usando StandardScaler
- Criação de variáveis derivadas:
  - Spending_Income_Ratio
  - Income_Per_Age
  - Spending_Per_Age
- Categorização de idade e renda

### 3. Determinação do Número Ideal de Clusters
Utilizamos três métodos para determinar o número ideal de clusters:

#### Método do Cotovelo e Silhouette Score
![Métodos de Avaliação](/images/metodos_avaliacao.png)

O gráfico acima mostra:
- **Método do Cotovelo (esquerda)**: 
  - Análise da inércia para K de 2 a 10
  - Identificação do ponto de cotovelo em K=4
  - Redução significativa da inércia até K=4

- **Silhouette Score (direita)**:
  - Melhor score obtido com K=4 (0.4158)
  - Boa separação entre clusters
  - Validação da escolha do número de clusters

#### Análise Visual dos Clusters
![Visualização dos Clusters](/images/clusters_visualization.png)

A visualização acima mostra a distribuição dos clusters para diferentes valores de K:
- **K=3**: Separação inicial clara dos grupos
- **K=4**: Melhor separação com grupos bem definidos
- **K=5**: Início de sobreposição e grupos menos distintos

Esta análise visual confirma que K=4 oferece a melhor segmentação dos dados, com clusters bem definidos e significativos.

### 4. Análise dos Clusters

#### Cluster 0 - "Conservadores Maduros" (52%)
- Idade mais elevada
- Renda e gastos abaixo da média
- Comportamento de consumo conservador

#### Cluster 1 - "Profissionais Equilibrados" (36.5%)
- Idade abaixo da média
- Boa renda
- Gastos moderadamente altos

#### Cluster 2 - "Jovens Alto Consumo" (11.5%)
- Muito jovens
- Renda baixa
- Gastos muito altos

## 💡 Insights e Recomendações

### Estratégias de Marketing

#### Para Conservadores Maduros:
- Programa de fidelidade com benefícios de longo prazo
- Comunicação tradicional e formal
- Ênfase em segurança e confiabilidade

#### Para Profissionais Equilibrados:
- Programa de benefícios premium
- Marketing digital profissional
- Produtos e serviços exclusivos

#### Para Jovens Alto Consumo:
- Programa gamificado
- Marketing em redes sociais
- Ofertas relâmpago e tendências

### Oportunidades Identificadas
1. Cross-Selling entre clusters
2. Programa de indicação personalizado
3. Experiência omnichannel adaptada
4. Desenvolvimento de produtos específicos
5. Gestão de risco por perfil

## 📈 Implementação e Monitoramento

### KPIs Sugeridos
- Taxa de conversão por cluster
- Ticket médio
- Frequência de compra
- Lifetime Value (LTV)
- NPS (Net Promoter Score)

### Ciclo de Atualização
- Revisão trimestral da segmentação
- Ajuste contínuo das estratégias
- Monitoramento de migração entre clusters

## 🔧 Tecnologias Utilizadas
- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- NumPy

## 📚 Bibliotecas Necessárias
```python
import pandas as pd
import numpy as np
from sklearn.cluster import KMeans
from sklearn.preprocessing import StandardScaler
import matplotlib.pyplot as plt
import seaborn as sns
```

## 🚀 Como Executar o Projeto

### Estrutura do Projeto
```
kmeans-customer-segmentation/
│
├── data/
│   └── Mall_Customers.csv
│
├── images/
│   ├── exploratory_analysis.png
│   ├── correlation_matrix.png
│   ├── metodos_avaliacao.png
│   └── clusters_visualization.png
│
├── notebooks/
│   └── customer_segmentation_analysis.ipynb
│
├── README.md
└── requirements.txt
```

### Passos para Execução
1. Clone o repositório
2. Crie um ambiente virtual (recomendado):
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   # ou
   venv\Scripts\activate  # Windows
   ```
3. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```
4. Execute o Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
5. Abra o notebook `customer_segmentation_analysis.ipynb`
6. Execute as células em ordem

## 📊 Resultados e Métricas
- Silhouette Score: 0.4158 (K=4)
- Distribuição equilibrada dos clusters
- Segmentação clara e acionável
- Estratégias de marketing personalizadas

## 🔄 Próximos Passos
1. Implementar sistema de monitoramento contínuo
2. Desenvolver campanhas piloto por cluster
3. Criar dashboard de acompanhamento
4. Estabelecer processo de feedback
5. Refinar estratégias baseado em resultados

## 👥 Autores
Victor Prada
