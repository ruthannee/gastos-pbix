# gastos-pbix

## Informações exibidas:
* GASTOS: total de gastos (soma);
* MÉDIA: média de gastos (média);
* COMPRAS: quantidade de compras realizadas (contagem);
* DIAS: quantidade de dias que as compras foram realizadas (contagem distinta);
* GASTO POR PERÍODO: série temporal (gráfico de linha);
* GASTO POR DIA DA SEMANA: soma dos gastos por dia, em gráfico de barras;
* GASTO POR CATEGORIA: gasto representado por frequências em eixo horizontal (gráfico de barras horizontais);
* CONTAGEM DE GASTO POR CATEGORIA: contagem das categorias representada por nuvem de palavras;
* ATT: medida que exibe a última atualização do dashboard.

### Segmentação de dados:
* FILTRO POR ANO;
* FILTRO POR MÊS.

## Formatação das features
### - DATE
* Conversão dos dados para o tipo DATA;
* Transformação das datas em dias da semana (em colunas numérica e nominal);

### - CATEGORY
* Formatação UTF-8;

### - AMOUNT
* Transformação dos dados em números decimais;
* Remoção dos valores vazios.

## Carga
* Feature "amount" com valores maiores que zero;
* Ordenação da feature nominal dos dias da semana com base na feature numérica;
* Aplicação da moeda (R$) para os valores da feature "amount".
