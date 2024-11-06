# Let's Snack - Inteligência Artificial

## Descrição

Esta IA foi projetada para identificar e classificar perfis de usuários com base em seus hábitos alimentares e suas características físicas, usando técnicas de aprendizado de máquina supervisionado e não supervisionado. A IA é capaz de prever o nível de alinhamento de um usuário com o perfil ideal, baseando-se em fatores como IMC, frequência de exercícios e consumo de determinados tipos de alimentos.

### Análise Exploratória e Pré-Processamento de Dados

A IA realiza uma Análise Exploratória de Dados (AED) detalhada para garantir que os dados estejam limpos e prontos para serem processados. A análise inclui:

- **Limpeza e normalização dos dados**: Variáveis como idade, altura e peso foram ajustadas para evitar ruídos e inconsistências. Outliers foram tratados para melhorar a precisão dos modelos.
- **Seleção de features**: Foram selecionadas as variáveis mais relevantes para o modelo, como altura e peso, que têm forte correlação com o estado nutricional.
- **Redução de dimensionalidade**: Ferramentas como PCA e SelectKBest foram aplicadas para simplificar o conjunto de dados, reduzindo o número de variáveis e mantendo apenas aquelas que mais contribuem para a previsão.

### Modelos Supervisionados

Três modelos supervisionados foram testados:

- **Naive Bayes**: Usado para comparar com os demais, apresentou uma performance média devido à suposição de independência das variáveis.
- **Decision Tree**: Demonstrou alta precisão e foi eficaz em lidar com variáveis categóricas e numéricas, fornecendo bons resultados em previsões mais complexas.
- **K-Nearest Neighbors (KNN)**: Esse modelo obteve o melhor desempenho, com alta acurácia, especialmente ao usar altura e peso como features principais.

### Modelos Não Supervisionados

Para complementar as análises, um modelo de clustering (K-means) foi aplicado com o objetivo de agrupar os usuários em clusters baseados em seus hábitos alimentares:

- **Clusters de hábitos alimentares**: O K-means identificou diferentes perfis de saúde e estilo de vida, que ajudam a categorizar os usuários conforme seus comportamentos e preferências. Os clusters refletem desde usuários com hábitos extremamente saudáveis até aqueles que apresentam padrões de comportamento com riscos à saúde, como alta ingestão de fast food e baixo nível de atividade física.

---
## Dependências

Para executar este projeto, você precisará instalar as seguintes bibliotecas e ferramentas:

### Python

- Python 3.12 ou superior
- pandas
- plotly
- matplotlib
- seaborn
- numpy
- scipy
- statsmodels
- scikit-learn
- yellowbrick
- optuna

---

Você pode instalar as dependências Python com o seguinte comando:

```bash
pip install -r requirements.txt
```

## Autores

- [@EnzoHino](https://www.github.com/EnzoHino)
- [@ArthurMicarelli](https://github.com/ArthurMicarelli)
