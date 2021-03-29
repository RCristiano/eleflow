# Questões

## 1 - MIGRAÇÃO DE DADOS

### Quais das ferramentas listadas ao lado você utilizaria para fazer a migração de um banco de dados Oracle on premises para um Azure SQL DB? Leve em consideração que você só possui acesso de leitura no servidor Oracle on premises. Explique brevemente quais as ferramentas e passos necessários para essa migração.

* [ ] Databricks
* [X] Data Factory
* [ ] SQL Server Migration Assistant (SSMA)
* [ ] Dataflow
* [ ] Event Hubs

R: O SSMA poderia ser usado se o servidor Oracle possui-se acesso de escrita porque precisa de acesso para instalação de extensões, porém sem o acesso o Data Factory é mais interessante, pois não necessita do acesso de escrita e possibilita cópia paralela entre os databases.

> fontes: https://docs.microsoft.com/en-us/sql/ssma/oracle/migrating-oracle-data-into-sql-server-oracletosql?view=azuresqldb-current
https://docs.microsoft.com/en-us/azure/data-factory/connector-oracle

## 2 - SQL

### Em termos de performance, qual(is) dos joins listados ao lado não é(são) o(s) mais recomendado(s) e por quê?

* [ ] inner join
* [ ] left outer join
* [X] cross join
* [ ] full outer join
* [ ] right join

R: Em termos de performance o cross join é o menos recomendado pois executa uma comparação NxN.

## 3 - DADOS

### Qual a diferença entre um dado estruturado e um dado não-estruturado? Como você armazenaria cada um deles? (liste mais de uma opção para cada tipo de dado).

R: Dados estruturados são organizado de forma rígida com estruturas previamente definidas e planejadas para o armazenamento, enquanto dados não estruturados são flexíveis e não dependem de uma estrutura rígida ou predefinida, dados estruturados podem ser armazenados em SGDBs como PostgreSQL, MYSQL ou SQL Server, porém dados não estruturados podem ser armazenados em Object Storages como HDFS e o Azure Blob Storage. Existem ainda os dados semi estruturados que possuem estruturas dinâmicas ou esquemas predefinidos porém flexíveis que podem ser armazenados como dados não estruturados ou  em sistemas como MongoDB, ElasticSearch ou o Azure CosmosDB sendo estes bancos de dados não relacionais também conhecidos pela sigla NoSQL.
