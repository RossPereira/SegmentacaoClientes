# Problema de Negócio e Solução:

**Problema de Negócio: A Black Friday está chegando e a empresa gostaria de ter um melhor resultado em suas campanhas de marketing nesse ano, porém, o setor de marketing determinou que as campanhas devem ser o mais personalizadas possível para cada grupo de cliente aumentando assim a conversão.** 

**Solução proposta:** Será construido um modelo de Machine Learning de clusterização para divisão dos clientes na base em grupos(clusters) para que assim a empresa possa direcionar campanhas de marketing específicas para cada grupo de acordo com as características do grupo para aumentar a conversão da campanha de Black Friday.

# Bibliotecas Usadas:

* Scikit learn
* Pandas
* Numpy
* Seaborn
* MatPlotLib

# Técnicas de Machine Learning:

* Algoritmos de Cluesterização (K-Means)
* Método de Elbow para definição dos Cluesters
* Padronização dos dados (StandardScaler)
* Tipo de Aprendizagem: Não supervisionada

# Construção:

Após a coleta dos dados foi feita a análise exploratória e estatística para entendermos melhor o comportamento da base.

Na fase de pré-processamento foi feita a verificação de valores nulos e vazios existiam 313 Registros nulos na base de dados na categoria Pagamento Mínimo e 1 Registro na categoria Limite de Crédito, a estratégia escolhida para substituição desses valores foi utlizar a média. após foi feita a verificação de valores duplicados na base mas não encontramos nenhum registro. Foi feita também a padronização dos dados.

Como a empresa não tinha uma ideia do número de grupos em que desejava dividir os clientes, utilizei o método Elbow para definir o número ideia de clusters, e utilizei o algoritmo K-Means, que por sem um algoritmo de aprendizado não supervisionado, gerou a divisão em cluster automaticamente através da análise de atributos similares entre os registros. Aplicando o método chegou-se ao número de 8 clusters. O resultado foi transformado em um dataframe para visualização. Após foi feita uma análise junto com gestores da área de marketing para determinar as características de grupos mais relevantes para a empresa.
