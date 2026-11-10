# 📘 Atividade: Building REST APIs with FastAPI

## 🎯 Objetivo

Construa uma API REST para cadastrar e consultar livros usando FastAPI. Pratique criação de rotas, validação de dados com modelos Pydantic e uso de métodos e códigos de status HTTP.

## 📝 Tarefas

### 🛠️ Criar a primeira rota

#### Descrição
Crie uma aplicação FastAPI e implemente um endpoint simples para verificar se a API está funcionando.

#### Requisitos
O programa concluído deve:

- Criar uma instância de `FastAPI` em `main.py`.
- Implementar uma rota `GET /health` que retorne um JSON indicando que o serviço está ativo.
- Permitir iniciar a aplicação com Uvicorn e acessá-la pelo navegador.
- Disponibilizar a documentação interativa gerada pelo FastAPI em `/docs`.

### 🛠️ Cadastrar e listar livros

#### Descrição
Expanda a API para cadastrar livros e retornar a coleção. Use um modelo Pydantic para validar os dados recebidos e mantenha os registros em memória durante a execução.

#### Requisitos
O programa concluído deve:

- Definir um modelo de livro com `title`, `author` e `year`.
- Implementar `POST /books` para validar e cadastrar um livro, retornando o registro criado com status HTTP `201`.
- Implementar `GET /books` para retornar todos os livros cadastrados.
- Rejeitar dados inválidos usando a validação do FastAPI e do Pydantic.

### 🛠️ Consultar, atualizar e remover livros

#### Descrição
Complete a API permitindo localizar um livro pelo seu identificador, atualizar seus dados e removê-lo da coleção.

#### Requisitos
O programa concluído deve:

- Atribuir um identificador único a cada livro cadastrado.
- Implementar `GET /books/{book_id}` e retornar status HTTP `404` quando o livro não existir.
- Implementar `PUT /books/{book_id}` para atualizar um livro existente.
- Implementar `DELETE /books/{book_id}` para remover um livro existente.
- Testar as rotas pela documentação interativa em `/docs`, incluindo os casos de sucesso e de livro não encontrado.