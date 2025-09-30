# Data Pipeline com PySpark: Vendas e Cotações

Este projeto tem como objetivo aplicar técnicas de **engenharia e análise de dados com PySpark**.  
A proposta consiste em processar dados de vendas e cotações a partir de arquivos CSV brutos, realizando:

- Limpeza e padronização de informações (datas, acentos, nomes de cidades);
- Criação de DataFrames estruturados;
- Unificação de tabelas de vendas e cotações;
- Cálculo de métricas de negócio, como total de vendas, itens cotados e taxa de conversão por local;
- Armazenamento otimizado dos dados em formato Delta.

O projeto demonstra habilidades em **processamento de dados em larga escala, transformação, análise e persistência** usando PySpark.

---

## 🔧 Tecnologias Utilizadas

- Python 3.x  
- Apache Spark (PySpark)  
- Delta Lake  
- Spark SQL  

---

## 📂 Estrutura do Projeto

- **vendas.csv** → Arquivo bruto de vendas.  
- **cotacoes.csv** → Arquivo bruto de cotações.  
- **pipeline.py** → Script PySpark que realiza todo o processamento, unificação, análises e salvamento dos dados.  

> Obs: Os dados originais **não estão inclusos** no repositório.  
> Caso queira executar o projeto, crie arquivos `vendas.csv` e `cotacoes.csv` seguindo os schemas abaixo.

---

## 📊 Funcionalidades do Projeto

- **Limpeza e padronização de dados**  
  - Remoção de acentos, espaços e inconsistências.  
  - Correção de nomes de cidades e datas.  

- **Transformação**  
  - Criação de DataFrames estruturados a partir de arquivos CSV brutos.  
  - Conversão de colunas para tipos adequados (`int`, `double`, `date`).  

- **Unificação**  
  - Junção das tabelas de vendas e cotações com base em chaves comuns (`revendedor_id`, `local`, `tipo_maquina`).  

- **Análises realizadas**  
  - Total de vendas por local.  
  - Número de itens cotados por local.  
  - Taxa de conversão (cotações → vendas) por local.  

- **Persistência**  
  - Armazenamento otimizado em formato Delta Lake.  
