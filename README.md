# Análise de Risco de Crédito - Artigo IEEE

Este repositório contém os códigos, dataset e resultados utilizados no artigo científico **"Análise Comparativa de Algoritmos de Machine Learning para Classificação de Risco de Crédito"**.

O projeto compara a eficácia de algoritmos Random Forest e Redes Neurais (MLP) na detecção de inadimplência em clientes bancários.

## Metodologia e Técnicas Aplicadas

* **Pré-processamento de Dados:**
    * Limpeza e remoção de identificadores.
    * *Label Encoding* para variáveis categóricas.
    * **Padronização (StandardScaler):** Normalização das features para garantir a convergência otimizada da Rede Neural.
* **Validação Robusta:**
    * **Validação Cruzada Estratificada (Stratified K-Fold):** Aplicação de 5 dobras (folds) para mitigar o viés de seleção e garantir a consistência estatística dos resultados.
    * **Holdout:** Divisão final de 80/20 para teste cego.
* **Modelagem:**
    * Random Forest Classifier (100 estimadores).
    * Multilayer Perceptron (MLP) Neural Network (Arquitetura: 100x50 neurônios).

##  Como Executar

### Pré-requisitos

* **pip install pandas numpy scikit-learn matplotlib seaborn openpyxl

Executando a AnálisePara rodar o experimento e gerar os gráficos:Bashpython analise_credito.py

