# 📊 Telecom X – Análise de Evasão de Clientes

## 📌 Descrição do Projeto
Este projeto é parte do **Challenge Telecom_X_BR**, que tem como objetivo analisar e prever a **evasão de clientes (churn)** em uma empresa de telecomunicações.  
A base de dados utilizada contém informações contratuais, de serviços e de gastos dos clientes, permitindo identificar padrões e fatores que mais influenciam a decisão de encerrar o serviço.

---

## 🎯 Objetivos
- Explorar e compreender os dados de clientes.
- Identificar variáveis com maior impacto na evasão.
- Criar e comparar modelos de Machine Learning para previsão de churn.
- Propor ações estratégicas para redução da evasão.

---

## 📂 Estrutura do Projeto
1. **Pré-processamento dos Dados**
   - Remoção de colunas irrelevantes (`ID_Cliente`, `Tem_Internet`, `Qtd_Servicos`).
   - Transformação de variáveis categóricas via **One-Hot Encoding**.
   
2. **Análise Exploratória**
   - Proporção de clientes evadidos x ativos.
   - Balanceamento da base com **SMOTE** (oversampling da classe minoritária).
   - Matriz de correlação das variáveis.
   - Boxplots e scatter plots para variáveis como `Gastos_Totais` e `Meses_Contrato` versus evasão.

3. **Modelagem Preditiva**
   - Divisão em treino e teste (**70/30**).
   - **Modelo 1:** Regressão Logística (com normalização).
   - **Modelo 2:** Random Forest (sem normalização).
   - Avaliação usando métricas: Acurácia, Precisão, Recall, F1-score e Matriz de Confusão.

4. **Interpretação dos Modelos**
   - Coeficientes e *odds ratio* da Regressão Logística.
   - Importância das variáveis na Random Forest.
   - Comparação dos desempenhos.

5. **Relatório Final**
   - Apresentação dos principais fatores que influenciam a evasão.
   - Estratégias de retenção sugeridas.

---

## 🛠 Tecnologias Utilizadas
- **Python 3**
- **Bibliotecas**:
  - `pandas`, `numpy` – manipulação de dados
  - `matplotlib`, `seaborn` – visualização de dados
  - `scikit-learn` – machine learning e pré-processamento
  - `imblearn` – balanceamento de dados com SMOTE

---

## 📊 Principais Resultados
- **Variáveis mais associadas à evasão**: Tipo de contrato (*Month-to-month*), forma de pagamento (`Electronic check`), gastos totais e serviços adicionais.
- **Modelos Avaliados**:
  - Regressão Logística: bom desempenho e interpretabilidade.
  - Random Forest: melhor desempenho geral em termos de F1-score.
- **Acurácia e F1-score** acima de **82%** para ambos os modelos, com leve vantagem para Random Forest.

---

## 🚀 Como Executar o Projeto
Você pode executar no **Google Colab** ou localmente.

### Google Colab
1. Faça upload do arquivo CSV pré-processado.
2. Execute as células seguindo a ordem.
3. Ajuste os caminhos de leitura dos arquivos, se necessário.

## 📌 Próximos Passos e Melhorias
Testar outros algoritmos (XGBoost, LightGBM, SVM).
Implementar ajuste de hiperparâmetros (hyperparameter tuning).
Criar dashboard interativo para acompanhamento dos indicadores.
Avaliar impacto de campanhas específicas de retenção na taxa de churn.

---

## 👤 Autor

Renato Silva de Macedo
