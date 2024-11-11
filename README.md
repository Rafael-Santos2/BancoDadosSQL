# Passo a passo: Criação de um banco de dados
 Tutorial de como criar um banco de dados SQL que organiza
as informações de 'livros', 'editora', 'autores e assuntos'.
Este guia será dividido em etapas para demonstrar desde a
criação de tabelas, chaves e até manipulação/consulta de dados.

## Resumo de uma estrutura SQL
*__CREATE__ para criar 'Banco de dados' ou 'Tabelas'
*__ALTER__ Modificar e alterar colunas
*__DROP__ Para remover tabelas e banco
*__INSERT__ Inserir os dados nas tabelas
*__UPDATE__ Atualiza registro
*__DELETE__ Remover registro
*__SELECT__ Para consultar e visualizar dados

## Passo 1: criação do Banco de Dados e das Tabelas
#### 1.1 Criando o DB

```
CREATE DATABASE biblioteca;
Use biblioteca;
```

### 1.2 Criando a tabela 'editora'
```
CREATE TABLE editora(
    id_editora INT PRIMARY KEY AUTO_INCREMENT,
    nome_editora VARCHAR(100) NOT NULL,
    pais VARCHAR(50)
);
```

#### 1.3 Criando a tabela 'autor'
```
CREATE TABLE autor(
    id_autor INT PRIMARY KEY AUTO_INCREMENT,
    nome_autor VARCHAR(200),
    data_nascimento DATE
);
```

#### 1.4 Criando a tebela 'assunto'
```
CREATE TABLE assunto (
    id_assunto INT PRIMARY KEY AUTO_INCREMENT,
    descricao_assunto VARCHAR(300) NOT NULL
);
```
