# 🚀 Telecom X - Parte 2  
## 📊 Previsão de Evasão de Clientes (Churn Prediction)

---

## 🎯 Propósito do Projeto

O objetivo principal deste projeto é desenvolver modelos preditivos capazes de identificar clientes com alta probabilidade de cancelamento (Churn), permitindo que a empresa Telecom X antecipe ações estratégicas de retenção.

A evasão de clientes representa um impacto direto na receita e na previsibilidade financeira. Utilizando técnicas de Machine Learning, buscamos transformar dados históricos em inteligência estratégica para apoiar decisões de negócio.

---

## 🧠 Problema de Negócio

A Telecom X enfrenta um aumento na taxa de cancelamento de clientes.  
Antecipar quais clientes têm maior risco de evasão permite:

- Criar campanhas personalizadas de retenção
- Reduzir custos com aquisição de novos clientes
- Melhorar a experiência do cliente
- Aumentar a previsibilidade da receita

---


## 📦 Base de Dados

Arquivo utilizado:
dados_tratados.csv



Contém:

- Variáveis demográficas
- Informações contratuais
- Dados financeiros
- Indicadores de uso
- Variável alvo: Churn (evasão)

---

## 🔎 Preparação dos Dados

### 📌 1. Classificação das Variáveis

As variáveis foram organizadas em:

**🔢 Numéricas**
- Tempo de contrato
- Valor mensal
- Total gasto
- Indicadores quantitativos

**🔠 Categóricas**
- Tipo de contrato
- Método de pagamento
- Plano contratado
- Serviços adicionais

---

### 📌 2. Tratamento Aplicado

- Remoção de identificadores (ex: `customerID`)
- Conversão de variáveis numéricas armazenadas como texto
- Aplicação de One-Hot Encoding para variáveis categóricas
- Garantia de que todas as variáveis fossem numéricas para modelagem

---

### 📌 3. Normalização

Foi aplicado **StandardScaler** nas variáveis numéricas para:

- Padronizar escalas
- Melhorar desempenho da Regressão Logística
- Reduzir influência de magnitude nas variáveis

---

### 📌 4. Separação Treino/Teste

- 70% dos dados para treino
- 30% para teste
- Separação estratificada para manter proporção de churn

---

## 🤖 Modelos Utilizados

Foram treinados três modelos de classificação:

### 🔵 1. Regressão Logística
- Modelo interpretável
- Excelente baseline
- Permite análise dos coeficientes

### 🌳 2. Random Forest
- Captura relações não lineares
- Fornece importância das variáveis
- Robusto contra overfitting

### 🟣 3. Gradient Boosting
- Modelo mais avançado
- Foco em melhorar erros iterativamente
- Alta performance preditiva

---

## 📈 Métricas Avaliadas

Para avaliar o desempenho, foram utilizadas:

- Acurácia
- Precisão
- Recall (fundamental para churn)
- F1-Score
- ROC-AUC

---

## 📊 Análise Exploratória (EDA)

Durante a análise foram gerados gráficos como:

- 📊 Distribuição da variável Churn
- 🔥 Matriz de correlação
- 📈 Curva ROC comparativa entre modelos
- 📦 Matriz de confusão
- 🌳 Importância das variáveis
- 📊 Distribuição das probabilidades previstas

---

## 🔍 Principais Insights Encontrados

- Clientes com menor tempo de contrato apresentam maior risco de evasão.
- Planos de maior valor possuem taxa de cancelamento mais elevada.
- Baixo engajamento está fortemente associado ao churn.
- Certos tipos de contrato oferecem maior retenção.

---

## 🏆 Melhor Modelo

O modelo com melhor desempenho foi:

👉 **Regressão Logística**

Ela apresentou:

🔹 Maior Recall → melhor capacidade de detectar clientes que realmente cancelam

🔹 Maior F1-Score → melhor equilíbrio entre Precisão e Recall

🔹 Maior ROC-AUC → melhor capacidade geral de separação

🔹 Maior Acurácia → melhor desempenho global

---

## 💡 Recomendações Estratégicas

Com base nos resultados, recomenda-se:

- Criar campanhas específicas para clientes novos
- Incentivar contratos de longo prazo
- Monitorar clientes com baixo uso
- Implementar alertas automáticos para clientes com alto risco

---

## ⚙️ Como Executar o Projeto

### 1️⃣ Instalar as bibliotecas necessárias:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```
### 2️⃣ Executar o Notebook:

```bash
Challenge_Telecom_X_Parte_2_Final.ipynb
```

Certifique-se de que o arquivo esteja no mesmo diretório:

```bash
dados_tratados.csv
```

---

## 🛠 Tecnologias Utilizadas

- Python

- Pandas

- NumPy

- Matplotlib

- Seaborn

- Scikit-Learn

---

## 📌 Conclusão

Este projeto demonstra como técnicas de Machine Learning podem ser aplicadas para resolver problemas reais de negócio.

A previsão de churn permite que a Telecom X:

- Reduza perdas financeiras
- Aumente retenção de clientes
- Tome decisões orientadas por dados
- Ganhe vantagem competitiva

---

---

## 👤 Autor

**Fabio Zinetti**

* **GitHub:** [github.com/fabinhoz](https://github.com/fabinhoz/)
* **Projeto:** Desenvolvido como **parte 2** do **Challenge de Data Science – Alura**.

---

*Este projeto foi realizado com fins de estudo e prática de análise de dados aplicada a problemas de negócio reais.*
