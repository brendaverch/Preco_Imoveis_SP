<h1 align="center">:file_cabinet: Previsão de preços de imóveis em São Paulo</h1>

## :memo: Descrição
O projeto visa desenvolver um modelo de estimação de preços de imóveis na região de São Paulo. Em vez de se basear apenas nos bairros, o modelo utiliza regiões censitárias para uma previsão mais precisa e realista, uma vez que o valor de um imóvel muitas vezes é mais influenciado pela região em que está localizado do que pelo bairro em si.

Para alcançar essa precisão, o projeto integra dados de diversas fontes do IBGE, combinando informações essenciais de quatro tabelas distintas. A primeira tabela contém dados de preços e metragens, permitindo calcular o preço por metro quadrado. A segunda tabela fornece informações sobre as regiões censitárias, enquanto a terceira, através de manipulações e combinação com a primeira tabela, associa essas regiões aos dados de preço. Além disso, a quarta tabela traz informações geográficas essenciais.

Após a integração e o tratamento desses dados, obtém-se a base consolidada "dados_vendas_censo.csv".

Para encontrar o modelo mais adequado aos dados, foram testados três algoritmos de machine learning: regressão linear, árvore de decisão e random forest. A avaliação dos modelos foi realizada utilizando métricas como o Coeficiente de Determinação (R²) e o Erro Médio Absoluto (MAE). Após a avaliação, identificou-se que o modelo de random forest apresentou o melhor desempenho em termos de precisão e capacidade de generalização para a estimação de preços de imóveis neste contexto específico.

## :books: Funcionalidades
* Estimativa de Preços de Imóveis: O projeto permite estimar os preços de imóveis na região de São Paulo com base em dados de regiões censitárias, levando em consideração diversos fatores como metragem, localização e características geográficas.
* Integração de Dados: Realiza a integração de informações de diferentes fontes do IBGE, incluindo dados de preços, regiões censitárias e informações geográficas, para criar uma base de dados unificada para análise e modelagem.
* Pré-processamento de Dados: Executa manipulações e tratamentos nos dados brutos, incluindo limpeza, transformação e combinação de conjuntos de dados, para prepará-los para a construção de modelos de machine learning.
* Modelagem de Machine Learning: Utiliza algoritmos de regressão linear, árvore de decisão e random forest para construir modelos de estimação de preços de imóveis, permitindo uma análise comparativa de diferentes abordagens de aprendizado de máquina.
* Avaliação de Modelos: Avalia o desempenho dos modelos utilizando métricas como R² e erro médio absoluto (MAE), fornecendo insights sobre a precisão e a capacidade de generalização dos modelos.
* Seleção do Melhor Modelo: Identifica o modelo de random forest como o mais adequado para a estimação de preços de imóveis com base nos resultados da avaliação de desempenho.

## :wrench: Tecnologias utilizadas
* Análise de Dados:
   * Python
   * Pandas
   * NumPy
   * Seaborn
   * Matplotlib
   * Shapely
   * Geopandas
* Predição:
   * Python
   * Pandas
   * Seaborn
   * Matplotlib
   * NumPy
   * Scikit-learn (para regressão linear, árvore de decisão e random forest)
   * Joblib

## :rocket: Rodando o projeto
Para rodar o repositório é necessário clonar o mesmo, dar o seguinte comando para iniciar o projeto:
```
<pip install pandas numpy seaborn matplotlib shapely geopandas scikit-learn joblib>
```
