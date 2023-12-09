# Projeto-Execução-Financeira
ETL/pgAdmin/Power B.I
<div align="center">
	
![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white) ![Power Bi](https://img.shields.io/badge/power_bi-F2C811?style=for-the-badge&logo=powerbi&logoColor=black) ![SQL](https://img.shields.io/badge/SQL-%2300758F.svg?style=for-the-badge&logo=sql&logoColor=white) ![ETL](https://img.shields.io/badge/ETL-pink?style=for-the-badge&logo=sql&logoColor=white)


</div>
<br>




# PROJETO CRIAÇÃO DATA BASE, DATA WAREHOUSE E DASHBOARD



OBJETIVO:
    
   - Análisar as informações contidas no banco de dados, denominado execução_financeira proposto.
   - Realizar a análise exploratória dos dados inseridos; elimando nulls, ajustando valores e datas para melhor análise e lisura dos dados.
   - Tratar os dados, fazendo as devidas correções e em acordo com o processo de ETL o qual fora aplicado no decorrer da unidade.
   - Criar um Dashboard para melhor visualização das informações contidadas no DW utilizando ferramenta de visualização de dados.
      
MODELAGEM LÓGICA, CONCEITUAL E DIMENSIONAL:
LÓGICA:
CONCEITUAL:
DIMENSIONAL:

# Ainda irão ser inseridos;






# ETAPA - MODELAGEM DOS SCRIPTS PARA CRIAÇÃO DAS SEGUINTES TABELAS: DIMENSÃO E FATO

* PARA AS TABELAS FORAM UTILIZADAS A MESMA METODOLOGIA, PRIMEIRO FORAM CRIADOS OS RESPECTIVOS SELECTS PARA TRAZER OS CAMPOS NECESSÁRIOS PARA CRIAÇÃO DAS TABELAS.
* APÓS EXECUÇÃO DO SELECT FORAM VERIFICADOS OS RESULTADOS.
* INCLUÍDA A PRIMEIRA LINHA CREATE TABLE AS 'NOME_TABELA', PARA TAL FUNCIONALIDADE.
* A CRIAÇÃO SEMPRE DEVE SER FEITA EM 'DATA_WAREHOUSE', LOCAL ONDE ESTÁ O DW, COMO VIMOS DURANTE O CURSO E TAMBÉM PARA PRESERVAÇÃO DA BASE REAL, ANTES DE RECEBER O TRATAMENTO, DEVEREMOS REALIZAR A CRIAÇÃO DO DW.

Sintetizando do ponto de vista de dados, realizamos os seguintes comandoa abaixo:

Criação e reorganização do banco de produção:
Create table ods.financeiro as 
select * from execucao_financeira_despesa

-------------------------------------
Selecionar todos os dados:

Select * 
from ods.financeiro

--------------------------------------

# TABELA DIM_ORGAO


Na análise exploratória foi indentificado orgãos com o mesmo código de orgão porém descrições diferentes. Utilizamos o select abaixo para identificar quais eram:

Select codigo_orgao, dsc_orgao
From execucao_financeira_despesa






