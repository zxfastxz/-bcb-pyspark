# Análise de Dados da API do Banco Central com PySpark

Este projeto utiliza um dos recursos da API pública do Banco Central do Brasil para coletar e transformar dados econômicos usando PySpark.

##  Objetivo
Aplicar pelo menos 5 operações de **Transformação** e **Ação** em uma base de dados retornada da API, conforme solicitado na atividade acadêmica.

##  API utilizada
`https://api.bcb.gov.br/dados/serie/bcdata.sgs.24363/dados?formato=json](https://olinda.bcb.gov.br/olinda/servico/MPV_DadosAbertos/versao/v1/"
    "odata/Quantidadeetransacoesdecartoes(trimestre=@trimestre)?@trimestre='2024'"
    "&$top=100&$format=json&$select=trimestre,nomeBandeira,"
    "qtdCartoesEmitidos,qtdCartoesAtivos,valorTransacoesNacionais`

Essa API retorna dados de uma série temporal do Banco Central.

##  Operações aplicadas
- Transformações:
  - Conversão de tipos (`cast`)
  - Conversão de datas (`to_date`)
  - Extração de ano e mês
  - Agrupamento por ano com média (`groupBy + agg`)
- Ações:
  - Exibição de registros (`show`)
  - Contagem (`count`)
  - Exibição de médias anuais (`show`)

##  Tecnologias
- Python
- PySpark
- Pandas
- Google Colab

##  Execução
1. Abra o notebook no Google Colab.
2. Execute todas as células sequencialmente.
3. O resultado será exibido diretamente no notebook.
