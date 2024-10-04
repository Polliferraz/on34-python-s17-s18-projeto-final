README:
Projeto final
Queimadas no Brasil: 
Análise da Influência de Fatores Ambientais e Climáticas nos anos de 2022 e 2023

Nara Sane
Polli Ferraz
Reprograma - On34

Objetivo Geral:
Analisar a correlação entre a ocorrência de queimadas e fatores climáticos, como períodos sem chuva, precipitação, e a distribuição espacial das queimadas em diferentes biomas no Brasil, para os anos de 2022 e 2023.

Hipóteses:
Hipótese 1: Queimadas são mais frequentes em determinados biomas e variam de acordo com as estações do ano.
Objetivo: Analisar se há biomas ou regiões mais propensas a queimadas e como as estações do ano influenciam essa frequência.
Hipótese 2: A ocorrência de queimadas não tem influência do tamanho dos períodos de seca/sem precipitação.
Objetivo: Verificar a relação entre o número de dias sem chuva/precipitação e a quantidade de focos de queimadas.
Hipótese 3:A precipitação média diária não tem correlação com os focos de queimadas, entre 2022 e 2023.
Objetivo: Comparar a quantidade de focos de queimadas com a precipitação mensal, entre os anos de 2022 e 2023. 

Metodologia de Análise:
Google colab: importar os arquivos csv.
Concatenar as tabelas foco_br_ref (2022 e 2023)
Concatenar as tabelas qmd_inpe (2022, 2023)
Explorar as duas tabelas concatenadas  e juntá-las  em um único csv para iniciar as análises das hipóteses
Tratamento dos Dados:
Limpeza dos dados: Verificar e eliminar possíveis inconsistências nos dados, como duplicidades, dados negativos e dados ausentes.
Padronização dos dados: foram conferidos e padronizados os tipos de dados.
Criação de colunas novas: foram criadas três novas colunas, uma nomeada de  “Mês/Ano” a partir da coluna de “Data/Hora”, uma coluna “Estação” correspondentes a estação do período do mês/ano e uma coluna de “Região” a partir da coluna existente “Estado”.

Análise Descritiva:
Focos de queimadas por Bioma e Região;
Focos de queimadas por Mês e Bioma;
Focos de queimadas por Mês e Estação do Ano;
Focos de queimadas por Categoria de Seca e Ano;
Contagem de focos de queimadas por Categoria de Seca para cada bioma, por ano;
Contagem de focos de queimadas e Precipitação média diária mensal, por ano
Análise Estatística:
Análise de variância (ANOVA: oneway) entre os focos de queimadas e as estações;
Análise de variância (ANOVA: oneway entre os focos de queimadas e as Categoria de Seca;
Correlação de Pearson entre os focos de queimadas e a Precipitação média diária de cada mês;

Considerações finais
Hipótese 1: Foi verificado se há diferenças significativas nos focos de queimadas entre as estações do ano. Com uma Estatística F de 12,84 e Valor p de 0,0000669, rejeitamos a hipótese nula, concluindo que há diferenças significativas entre as estações, sugerindo que as condições climáticas influenciam as queimadas.
Hipótese 2: Não há diferença significativa (p>0,05) entre os focos de queimadas e os diferentes períodos de seca, em 2022; Há diferença significativa (p<0,05) entre os focos de queimadas e os diferentes períodos de seca, em 2023.
Hipótese 3: Não há correlação entre os focos de queimadas e a precipitação média diária, em ambos os anos (2022: r=-0,24, 2023: r=-0,44). E a relação de tais variáveis apresentou-se inversamente proporcional.

Fonte de dados:
Dados de queimadas disponibilizados pelo INPE:
Obtido em: https://terrabrasilis.dpi.inpe.br/queimadas/bdqueimadas/#exportar-dados
Disponível em: https://terrabrasilis.dpi.inpe.br/queimadas/bdqueimadas/#exportar-dados
