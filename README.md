# 🍎 Projeto Quitanda — MySQL

Este repositório contém meu primeiro projeto utilizando **MySQL**, criado durante meus estudos de banco de dados.  
Aqui pratico conceitos fundamentais como:

- Criação de banco de dados (DDL)
- Criação de tabelas
- Chave primária (PRIMARY KEY)
- Inserção de dados (DML)
- Seleção de dados com filtros (SELECT / WHERE)
- Atualização de informações (UPDATE)
- Exclusão de registros (DELETE)
- Alteração de estrutura de tabela (ALTER TABLE)

---

## 🗂️ Estrutura do Projeto

O arquivo principal é:

db_quitanda.sql 

Ele contém:

✔ Criação do banco db_quitanda
✔ Criação da tabela tb_produtos
✔ Inserção de vários produtos
✔ Consultas básicas
✔ Atualização de preços
✔ Exclusão de dados
✔ Alteração do tipo da coluna preco

📝 Principais Comandos Utilizados
🔹 Criação do banco e uso
CREATE DATABASE db_quitanda;
USE db_quitanda;

🔹 Criação da tabela
CREATE TABLE tb_produtos(
    id BIGINT AUTO_INCREMENT,
    nome VARCHAR(255) NOT NULL,
    quantidade INT,
    datavalidade DATE,
    preco DECIMAL NOT NULL,
    PRIMARY KEY (id)
);

🔹 Inserindo dados
INSERT INTO tb_produtos(nome, quantidade, datavalidade, preco) 
VALUES ("tomate",100, "2023-12-15", 8.00);

🔍 Consultas de exemplo
SELECT * FROM tb_produtos;
SELECT nome, preco FROM tb_produtos;
SELECT * FROM tb_produtos WHERE preco > 5;

🔧 Atualizando e excluindo dados
UPDATE tb_produtos SET preco = 2.99 WHERE id = 6;
DELETE FROM tb_produtos WHERE id = 2;

✨ Objetivo do Projeto

Este projeto tem como objetivo:

consolidar conhecimentos iniciais em SQL

treinar comandos DDL e DML

aprender a manipular tabelas reais

entender como funciona um CRUD simples em banco de dados

🚀 Próximos Passos

Criar uma tabela de categorias

Relacionar produtos com categorias (FOREIGN KEY)

Criar consultas com JOIN

Criar mais tabelas e relacionamentos

📚 Tecnologias

MySQL 8.x

MySQL Workbench

Git / GitHub

💡 Observação

Este é meu primeiro projeto com SQL — ele será atualizado conforme meu aprendizado evolui.