# Banco 1

# exercicio 1

```sql
-- criar tabela de Clientes

create table Clientes(
id_cliente int primary key AUTO_INCREMENT,
nome_cliente varchar(100),
email_cliente varchar(150),
data_nascimento date,
telefone_cliente varchar(15)
);
```

# exercicio 2

```sql
--criar tabela de Produtos

create table Produtos(
id_produto int primary key,
nome_produto varchar(100) NOT NULL UNIQUE,
preço_produto decimal(8,2)
);
```

# exercicio 3

```sql
--criar tabela de Faturas

create table Faturas(
id_fatura int primary key,
data_criaçao timestamp default current_timestamp,
valor_fatura decimal(10,2)
);
```
# exercicio 4
```sql
-- criar o banco de dados
create database bancoteste;
-- usar o banco escolhido
use bancoteste;
```
```sql
-- Crie uma tabela chamada "Funcionarios" com os campos ID (chave primária), Nome, Sobrenome e Salário.
create table Funcionarios(
id_funcionario int primary key,
nome varchar(100),
sobrenome varchar(100),
salario double
);
```
```sql
-- Adicione uma coluna chamada "DataNascimento" à tabela "Funcionarios" para armazenar a data de nascimento dos funcionários.
alter table Funcionarios add DataFuncionario date;
```
```sql
-- Crie uma nova tabela chamada "Departamentos" com os campos ID (chave primária) e Nome.
create table Departamentos(
id_departamentos int primary key,
nome varchar(100)
);
```
```sql
-- Adicione uma coluna chamada "IDDepartamento" à tabela "Funcionarios" para associar cada funcionário a um departamento.
alter table Funcionarios add IDDepartamento int;
```
```sql
-- Crie uma tabela chamada "Projetos" com os campos ID (chave primária) e NomeProjeto.
create table Projetos(
id_projeto int primary key,
nomeProjeto varchar(100)
);
```
```sql
-- Crie uma tabela chamada "Alocacoes" com os campos ID (chave primária), IDFuncionario e IDProjeto.
create table Alocacoes(
id_alocacoes int primary key
);
```
```sql
-- Renomeie a coluna "Sobrenome" da tabela "Funcionarios" para "Apelido".
alter table Funcionarios rename column sobrenome to apelido;
```
```sql
-- Crie uma tabela chamada "Clientes" com os campos ID (chave primária) e NomeCliente
create table Clientes(
id_cliente int primary key,
nomeCliente varchar(100)
);
```
```sql
-- Adicione uma coluna chamada "IDCliente" à tabela "Projetos" para associar cada projeto a um cliente.
alter table Projetos add IDCliente int;
```
```sql
-- Crie uma tabela chamada "Enderecos" com os campos ID (chave primária), Rua, Cidade e CEP.
create table Endereços(
id_endereço int primary key,
rua varchar(50),
cidade varchar(50),
CEP int(8)
);
```
```sql
-- Adicione uma coluna chamada "IDEndereco" à tabela "Funcionarios" para armazenar o endereço de cada funcionário.
alter table Funcionarios add IDEndereço int;
```
```sql
-- Renomeie a coluna "NomeCliente" da tabela "Clientes" para "NomeEmpresa".
alter table Clientes rename column nomeCliente to NomeEmpresa;
```
```sql
-- Crie uma tabela chamada "Pedidos" com os campos ID (chave primária) e DataPedido.
create table Pedidos(
id_pedidos int primary key,
dataPedido date
);
```
```sql
-- Adicione uma coluna chamada "IDCliente" à tabela "Pedidos" para associar cada pedido a um cliente.
alter table Pedidos add IDCliente int;
```
```sql
-- Crie uma tabela chamada "ItensPedido" com os campos ID (chave primária), IDPedido ( e IDProduto.
create table ItensPerdidos(
id_ItensPerdidos int primary key
);
```
```sql
create table Produtos(
id_produto int primary key,
NomeProduto varchar(50),
QuantidadeProduto int,
ValorProduto double
);
```
```sql
-- Renomeie a coluna "NomeProduto" da tabela "Produtos" para "DescricaoProduto".
alter table Produtos rename column NomeProdutos to DescriçaoProduto;
```
```sql
-- Crie uma tabela chamada "Estoques" com os campos ID (chave primária) e Quantidade.
create table Estoques(
id_Produtos int primary key,
quantidade int
);
```
```sql
-- Adicione uma coluna chamada "IDProduto" à tabela "Estoques" para associar cada item de estoque a um produto
alter table Estoques add IDProduto int;
```
```sql
-- Crie uma tabela chamada "Vendas" com os campos ID (chave primária) e DataVenda.
create table Vendas(
id_vendas int primary key,
DataVenda date
);
```
```sql
-- Adicione uma coluna chamada "IDCliente" à tabela "Vendas" para associar cada venda a um cliente.
alter table Vendas add IDCliente int;
```
