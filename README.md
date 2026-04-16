# Challenge_ClickBus_FIAP_2025
Challenge para empresa ClickBus FIAP 2025

 **Objetivo do Projeto**
Desenvolver um modelo de aprendizado de máquina capaz de prever [insira aqui o seu target, ex: inadimplência/vendas] utilizando o algoritmo XGBoost, conhecido pela sua alta eficiência e precisão em dados estruturados.

 **Tecnologias e Ferramentas**
* Linguagem: Python

* Modelagem: XGBoost (Extreme Gradient Boosting)

* Manipulação de Dados: Pandas e NumPy

* Preprocessamento: Scikit-Learn (LabelEncoder, Train-Test Split)

* Métricas: Mean Squared Error (MSE) / Accuracy

 **Pipeline de Desenvolvimento**
* Tratamento de Dados: Conversão de variáveis categóricas em numéricas utilizando LabelEncoder, garantindo que o modelo interprete corretamente as features qualitativas.

* Arquitetura do Modelo: Implementação do Gradient Boosting, onde o modelo aprende de forma iterativa, corrigindo os erros das árvores anteriores para minimizar o resíduo final.

* Avaliação: Teste do modelo em dados inéditos (X_test) para validar a capacidade de generalização e evitar o overfitting.
