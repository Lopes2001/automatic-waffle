
CREATE DATABASE empresa;

\c empresa;


CREATE TABLE funcionarios (
    id serial PRIMARY KEY,
    nome VARCHAR(50),
    idade INT,
    salario DECIMAL(10, 2),
    cargo VARCHAR(50),
    data_contratacao DATE
);

CREATE TABLE departamentos (
    id serial PRIMARY KEY,
    nome_departamento VARCHAR(50),
    localizacao VARCHAR(100),
    numero_funcionarios INT,
    orcamento_anual NUMERIC(10, 2),
    data_criacao TIMESTAMP
);

INSERT INTO funcionarios (nome, idade, salario, cargo, data_contratacao) 
VALUES ('João Silva', 30, 5000.00, 'Analista de Sistemas', '2023-01-15');

INSERT INTO departamentos (nome_departamento, localizacao, numero_funcionarios, orcamento_anual, data_criacao)
VALUES ('TI', 'São Paulo', 25, 1000000.00, '2023-01-01');

