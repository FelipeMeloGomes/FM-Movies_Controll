# Movies Controll

<img src="Modelagem de dados.PNG" width="100%"/>

## Descrição

Este é um projeto para controle de filmes e séries, permitindo o gerenciamento de informações como tipo (filme ou série), nome, episódios totais, episódios atuais e última visualização.

## Objetivo

Este é um projeto pessoal criado para aprimorar habilidades em SQL, fornecendo um ambiente prático para praticar conceitos fundamentais enquanto gerencio minha coleção de filmes e séries.

## Funcionalidades

-   Criação, leitura, atualização e exclusão de filmes/séries.
-   Registro da última visualização de cada item.

## Pré-requisitos

-   Node.js instalado
-   MySQL ou outro banco de dados relacional

## Instalação

1. Clone o repositório:

```
git clone https://github.com/seu-usuario/movies-controll.git
```

2. Instale as dependências:

```
npm install
```

## Uso

1. Inicie o projeto:

```
npm start
```

2. Utilize as rotas para gerenciar os filmes/séries.

## Exemplos de Uso

### Criação de um filme

```sql
INSERT INTO movies(`id`, `type`, `name`, `total_ep`, `atual_ep`, `last_view`)
VALUES (1, 0, 'Friends', 10, 1, current_timestamp());

Criação de uma série

INSERT INTO movies(id, type, name, total_ep, last_view)
VALUES (2, 1, 'Avengers', NULL, current_timestamp());

Atualização da última visualização

UPDATE `movies`
SET `last_view` = '2021-11-07'
WHERE `movies`.`id` = 1;

Exclusão de um filme/série

DELETE FROM movies
WHERE id = 2;
```
