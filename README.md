# Sistema de Biblioteca

Projeto de modelagem de banco de dados desenvolvido no MySQL Workbench para representar um sistema simples de gerenciamento de biblioteca.

## 📚 Estrutura do Banco de Dados

O modelo é composto por três entidades principais:

### Aluno

Armazena os dados dos alunos cadastrados.

- RA
- Nome
- Curso

### Livro

Armazena as informações dos livros disponíveis na biblioteca.

- ISBN
- Nome
- Autor
- Páginas

### Empréstimo

Registra os empréstimos realizados pelos alunos.

- ID do empréstimo
- RA do aluno
- ISBN do livro
- Data do empréstimo
- Data de devolução

## 🔗 Relacionamentos

O sistema possui os seguintes relacionamentos:

- Um aluno pode realizar vários empréstimos.
- Um livro pode estar associado a vários empréstimos.
- Cada empréstimo está relacionado a um aluno e a um livro.

## 🗂️ Arquivos

- `biblioteca.mwb` - Modelo EER criado no MySQL Workbench.
- `biblioteca.sql` - Script SQL para criação do banco de dados.

## 🛠️ Tecnologias utilizadas

- MySQL Workbench
- MySQL
- SQL

## 📌 Modelo

O projeto utiliza chaves primárias e estrangeiras para garantir a integridade dos relacionamentos entre Aluno, Livro e Empréstimo.