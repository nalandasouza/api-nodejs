# Sistema de Gestão de Autores e Livros

Este projeto é uma aplicação Backend desenvolvida com Node.js, Express e MongoDB. Ele permite realizar operações CRUD (Criar, Ler, Atualizar, Excluir) para gerenciar informações sobre autores e livros. A aplicação também oferece funcionalidades de paginamento e filtragem de livros, bem como tratamento de erros personalizado.

## Funcionalidades
Autoria:

Cadastro, listagem, atualização e remoção de autores.

Livros:

Cadastro, listagem, atualização e remoção de livros.

Busca por filtros como título, editora, número de páginas e autor.

Paginação:

Paginação de resultados em listas de livros e autores.

Tratamento de Erros:

Erros personalizados para diferentes tipos de falhas (validação, recursos não encontrados, erros internos).

## Tecnologias Utilizadas
Node.js: Ambiente de execução para JavaScript no lado do servidor.

Express: Framework para construção de APIs RESTful.

MongoDB: Banco de dados NoSQL para armazenamento de dados.

Mongoose: ODM (Object Document Mapper) para MongoDB.

Dotenv: Carregamento de variáveis de ambiente.

Autopopulate (mongoose): Plugin que facilita o preenchimento automático de campos relacionados (por exemplo, ao buscar livros, os dados do autor são carregados automaticamente).

## Estrutura do Projeto
Configuração de Banco de Dados:

O banco de dados é configurado e conectado utilizando Mongoose.

Modelos:

Autor: Define o schema e a validação dos dados de autores.

Livro: Define o schema e validações dos dados dos livros, incluindo referência ao modelo de autor.

Controllers:

AutorController: Contém as funções responsáveis por manipular os dados dos autores.

LivroController: Contém as funções responsáveis por manipular os dados dos livros e realizar buscas filtradas.

Middlewares:

Paginação: Implementa a lógica de paginação para consultas.

Tratamento de Erros: Middleware global para tratamento de erros específicos, como erros de validação e recursos não encontrados.

Rotas: Define as rotas para autores e livros, conectando as funções dos controllers às operações HTTP (GET, POST, PUT, DELETE).

Servidor:

Configura a aplicação Express, conectando as rotas e tratando erros.

## Este projeto oferece uma API simples, porém robusta, para gerenciar livros e autores, com funcionalidades de busca avançada e tratamento de erros, sendo uma base sólida para a construção de sistemas mais complexos.
