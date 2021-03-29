# Questões

## 1 - MIGRAÇÃO DE DADOS

### Quais das ferramentas listadas ao lado você utilizaria para fazer a migração de um banco de dados Oracle on premises para um Azure SQL DB? Leve em consideração que você só possui acesso de leitura no servidor Oracle on premises. Explique brevemente quais as ferramentas e passos necessários para essa migração.

* [ ] Databricks
* [ ] Data Factory
* [ ] SQL Server Migration Assistant (SSMA)
* [ ] Dataflow
* [ ] Event Hubs

R:

> fontes: https://docs.microsoft.com/en-us/sql/ssma/oracle/migrating-oracle-data-into-sql-server-oracletosql?view=azuresqldb-current

## 2 - SQL

### Em termos de performance, qual(is) dos joins listados ao lado não é(são) o(s) mais recomendado(s) e por quê?

* [ ] inner join
* [ ] left outer join
* [X] cross join
* [ ] full outer join
* [ ] right join

R: Em termos de performance o cross join é o menos recomendado pois executa uma comparação NxN

## 3 - DADOS

### Qual a diferença entre um dado estruturado e um dado não-estruturado? Como você armazenaria cada um deles? (liste mais de uma opção para cada tipo de dado).

R: Dados estruturados são organizado de forma rigida com estruturas previamente definidas e planejadas para o armazenamento enquanto dados não estruturados são flexiveis e podem ter os dados
