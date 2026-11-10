# 📘 Atividade: Persistência de Dados com SQLite

## 🎯 Objetivo

Expanda a API de livros criada com FastAPI para armazenar os dados de forma permanente em um banco SQLite. Pratique criação de tabelas e consultas SQL parametrizadas usando o módulo `sqlite3` da biblioteca padrão do Python.

## 📝 Tarefas

### 🛠️ Criar o banco e a tabela de livros

#### Descrição
Configure a aplicação para criar um arquivo de banco de dados SQLite e uma tabela de livros quando iniciar. A inicialização não deve apagar os registros existentes.

#### Requisitos
O programa concluído deve:

- Usar o módulo `sqlite3`, sem depender de um servidor de banco de dados externo.
- Criar uma tabela `books` com `id`, `title`, `author` e `year`; usar `id` como chave primária autoincrementada.
- Garantir que o banco e a tabela sejam criados automaticamente quando ainda não existirem.
- Manter os dados existentes ao reiniciar a aplicação.

### 🛠️ Salvar e listar livros no banco

#### Descrição
Substitua o armazenamento em memória da API por operações no SQLite para cadastrar e listar livros.

#### Requisitos
O programa concluído deve:

- Persistir os livros enviados por `POST /books` na tabela `books`.
- Retornar o livro criado, incluindo seu identificador, com status HTTP `201`.
- Implementar `GET /books` usando os registros armazenados no banco.
- Usar parâmetros SQL (`?`) para inserir e consultar valores recebidos pela API.
- Confirmar as alterações no banco e fechar as conexões após as operações.

### 🛠️ Completar o CRUD e testar a persistência

#### Descrição
Conecte as rotas de consulta individual, atualização e remoção ao banco e verifique que os dados sobrevivem ao reinício da API.

#### Requisitos
O programa concluído deve:

- Implementar `GET /books/{book_id}`, `PUT /books/{book_id}` e `DELETE /books/{book_id}` usando o banco SQLite.
- Retornar status HTTP `404` quando uma rota solicitar um livro inexistente.
- Usar parâmetros SQL (`?`) para todos os valores fornecidos nas consultas pela API.
- Demonstrar que um livro cadastrado continua disponível após parar e iniciar a aplicação novamente.
- Testar pelo menos um fluxo de criação, consulta, atualização e remoção em `/docs`.
