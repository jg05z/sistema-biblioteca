# Sistema de Biblioteca

Projeto de modelagem de banco de dados desenvolvido no MySQL Workbench para representar o sistema de empréstimos de uma biblioteca universitária.

## 📚 Estrutura do Banco de Dados

O modelo é composto por quatro entidades principais:

### Aluno

Representa os alunos da instituição autorizados a realizar empréstimos.

- RA
- Nome
- E-mail
- Telefone

### Livro

Representa as publicações físicas disponíveis na biblioteca.

- ISBN
- Nome
- Autor
- Páginas

### Colaborador

Representa os funcionários autorizados a realizar os empréstimos.

- CPF
- Nome
- E-mail
- Cargo

### Empréstimo

Registra os empréstimos realizados no sistema.

- ID
- Data do empréstimo
- Data de devolução
- ISBN do livro
- CPF do colaborador

## 🔗 Relacionamentos

O modelo possui os seguintes relacionamentos:

- Um livro pode estar associado a vários empréstimos.
- Um colaborador pode registrar vários empréstimos.
- Cada empréstimo está relacionado a um livro e a um colaborador.

## 🔑 Chaves

As entidades utilizam chaves primárias e estrangeiras para garantir a integridade dos dados.

- `Aluno.ra` - Chave primária
- `Livro.isbn` - Chave primária
- `Colaborador.cpf` - Chave primária
- `Emprestimo.id` - Chave primária
- `Emprestimo.livroIsbn` → `Livro.isbn` - Chave estrangeira
- `Emprestimo.colaboradorCpf` → `Colaborador.cpf` - Chave estrangeira

## 🗂️ Arquivos

- `biblioteca.mwb` - Modelo EER desenvolvido no MySQL Workbench.
- `biblioteca.sql` - Script SQL para criação da estrutura do banco de dados.

## 🛠️ Tecnologias utilizadas

- MySQL Workbench
- MySQL
- SQL

## 📌 Objetivo

Desenvolver um Diagrama Entidade-Relacionamento (DER), definindo entidades, atributos, tipos de dados, chaves primárias, chaves estrangeiras e os relacionamentos necessários para representar a situação proposta.