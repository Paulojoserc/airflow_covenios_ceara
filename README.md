# Pipeline de Convênios do Ceará com Airflow

## O que é
Descrição curta: ETL diário dos convênios do Ceará Transparente para PostgreSQL, orquestrado pelo Apache Airflow.

## Arquitetura
Dois containers Docker (PostgreSQL e Airflow) na mesma rede.

## Pré-requisitos
Docker instalado.

## Passo a passo
1. Criar a rede
2. Subir o PostgreSQL
3. Criar banco, usuário e tabela
4. Subir o container do Airflow
5. Instalar o Airflow e o pandas
6. Copiar a DAG para o container
7. Acessar a interface em http://localhost:8080

## Como verificar
Ativar a DAG e rodar manualmente (Trigger).

## Problemas comuns
- "could not translate host name": containers fora da mesma rede.
- "password authentication failed": conferir usuário e senha.