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