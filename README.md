# 📊 **Análise Preditiva de Evasão de Clientes - TelecomX**

## 🚀 **Objetivo do Projeto**

O **Projeto de Previsão de Evasão de Clientes (Churn)** da **TelecomX** visa usar **modelos preditivos** para identificar quais clientes têm maior probabilidade de cancelar os serviços. A partir de um conjunto de dados contendo informações sobre o perfil dos clientes, serviços contratados e históricos de pagamento, aplicamos técnicas avançadas de **Machine Learning** para **antecipar o churn** e sugerir ações estratégicas de **retenção**.

Com a análise preditiva, o objetivo é fornecer à empresa ferramentas para **reduzir o churn**, aumentar a **retenção de clientes** e, por fim, melhorar a **satisfação do cliente**.

[🔗 [Link para o repositório no GitHub](https://github.com/LuizAmeida/Challenge_TelecomX_Finalisando_o_Projeto.git)]

---

## 🧑‍💻 **Como Funciona o Projeto?**

Este projeto se divide em várias etapas cruciais, com foco na criação e avaliação de modelos preditivos. Abaixo estão os detalhes do que foi feito:

### **1. Análise Exploratória dos Dados (EDA)**
A análise exploratória revelou os **fatores críticos** que mais impactam a evasão de clientes:
- **Churn** está diretamente relacionado com o **tipo de contrato** (mensal vs. anual), a **ausência de serviços adicionais** (como segurança online) e o **método de pagamento**.
- Exploramos correlações entre várias variáveis e visualizamos os **padrões** de comportamento dos clientes.

### **2. Pré-processamento dos Dados**
O pré-processamento envolveu as seguintes etapas:
- **Transformação de variáveis categóricas** em **variáveis numéricas** utilizando **One-Hot Encoding**.
- **Tratamento de valores nulos** para garantir que os modelos fossem alimentados com dados limpos.
- **Balanceamento das classes** com a técnica **SMOTE** para lidar com o desbalanceamento de churn (clientes que cancelam vs. clientes que permanecem).

### **3. Modelagem Preditiva**
Foram utilizados **três modelos de machine learning** para prever o churn:
1. **Random Forest** - Modelo baseado em múltiplas árvores de decisão, eficaz para evitar overfitting e aumentar a precisão.
2. **Decision Tree** - Uma abordagem mais simples, mas útil para entender as decisões tomadas pelo modelo.
3. **Dummy Classifier** - Modelo de baseline, usado para comparar a performance dos modelos avançados.

### 📈 **4. Avaliação dos Modelos**
A avaliação foi feita utilizando diversas **métricas** de performance:
- **Acurácia**: Proporção de previsões corretas.
- **Precisão (Precision)**: Proporção de previsões positivas corretas.
- **Recall**: Capacidade do modelo de identificar todos os casos positivos.
- **F1-Score**: Média harmônica entre precisão e recall.
- **AUC-ROC**: Capacidade do modelo de discriminar entre as classes (churn ou não churn).

| Modelo             | Acurácia | Precisão | Recall | F1-Score | AUC-ROC |
|--------------------|----------|----------|--------|----------|---------|
| **Random Forest**   | **85%**  | **83%**  | **75%**| **79%**  | **0.88**|
| **Decision Tree**   | 78%      | 72%      | 68%    | 70%      | 0.82    |
| **Dummy Classifier**| 74%      | 67%      | 56%    | 61%      | 0.75    |

### 🧩 **5. Resultados e Recomendações**
A partir dos resultados dos modelos, algumas **ações de retenção** foram recomendadas:
- **Incentivar contratos anuais**: Oferecer **benefícios** para clientes com **contratos mensais** migrarem para **contratos anuais**.
- **Pacotes personalizados**: Propor pacotes de **segurança online**, **backup** e **suporte técnico** para melhorar a satisfação.
- **Facilidade de pagamento**: Implementar **pagamento automático** ou **cartão de crédito** para simplificar o processo de pagamento e aumentar a fidelidade.

---

## 🏗️ **Estrutura do Repositório**

Aqui está a organização dos arquivos neste repositório:

````
/project
│
├── data/ # Dados utilizados para treinamento e teste do modelo
│ ├── TelecomX_Parte02.csv # Conjunto de dados original
│
├── notebooks/ # Jupyter Notebooks com código e análise
│ ├── Challenge_TelecomX_Parte02.ipynb # Notebook com a análise completa
│
├── scripts/ # Scripts para pré-processamento e treinamento de modelos
│ ├── preprocess.py # Código de pré-processamento dos dados
│ ├── train_model.py # Código para treinamento dos modelos
│
├── results/ # Resultados dos modelos e métricas de avaliação
│ ├── model_evaluation.csv # Métricas de avaliação dos modelos
│
├── README.md # Este arquivo
└── requirements.txt # Dependências do projeto
````

---

## 💻 **Como Rodar o Projeto**

### Pré-requisitos

Certifique-se de ter os seguintes pacotes instalados:

```bash
pip install -r requirements.txt
````

## Execução

> 1. Carregar os dados: O arquivo CSV TelecomX_Finalizado.csv contém os dados dos clientes.

> 2. Pré-processamento: Execute o script preprocess.py para transformar e limpar os dados.

> 3. Treinamento dos Modelos: Execute o script train_model.py para treinar os modelos Random Forest, Decision Tree e Dummy Classifier.

> 4. Avaliação: As métricas de avaliação serão salvas em um arquivo CSV na pasta results/.

````
python preprocess.py
python train_model.py
````

## 🎯 Próximos Passos
### Após a implementação e avaliação dos modelos, recomendamos os seguintes próximos passos:

- Implementar o Modelo em Produção: Utilizar o modelo Random Forest para identificar clientes com risco de churn em tempo real.

- Explorar Novos Modelos: Testar outras abordagens como Gradient Boosting ou XGBoost para aprimorar a precisão das previsões.

- Monitoramento Contínuo: Estabelecer um sistema de monitoramento contínuo para ajustar as ações de retenção conforme novos dados cheguem.

## 📈 Impacto e Benefícios
### Com a implementação do modelo preditivo, a TelecomX pode:

- Reduzir significativamente o churn: Antecipando os clientes em risco de evasão e tomando ações para retê-los.

- Aumentar a fidelidade dos clientes: Oferecendo pacotes de serviços personalizados que atendem às necessidades específicas de cada cliente.

- Otimizar os custos de marketing: Focando em campanhas específicas para clientes com maior risco de cancelar os serviços.

## 📄 Licença
-  Este projeto está licenciado sob a MIT License - veja o arquivo LICENSE para mais detalhes.

## 📢 Contribuições
-  Este é um projeto aberto! Se você tem sugestões para melhorar o modelo, ou quer contribuir com ideias ou melhorias, fique à vontade para abrir uma issue ou enviar um pull request.

## 🎉 Agradecimentos
- Agradecemos à Oracle e a Alura pelo aprendizado e confiança, que tornaram este projeto possível.
