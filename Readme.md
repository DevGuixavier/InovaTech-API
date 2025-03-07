# InovaTech API

Esta é a API do laboratório de criação de APIs da InovaTech. A API é construída usando Flask e inclui autenticação JWT e documentação Swagger.

## Estrutura do Projeto

O projeto está organizado da seguinte forma:

- `app.py`: Arquivo principal da aplicação Flask.
- `docker-compose.yml`: Arquivo de configuração do Docker Compose.
- `Dockerfile`: Arquivo de configuração do Docker.
- `Readme.md`: Documentação do projeto.
- `requirements.txt`: Lista de dependências do projeto.
- `static/`: Diretório contendo arquivos estáticos, incluindo a documentação Swagger.

## Configuração do Ambiente

### Requisitos

- Docker
- Docker Compose

### Instruções

1. Clone o repositório:
    ```sh
    git clone <URL_DO_REPOSITORIO>
    cd API
    ```

2. Construa e inicie os containers Docker:
    ```sh
    docker-compose up --build
    ```

3. Acesse a API em `http://localhost:1313`.

## Dependências

As dependências do projeto estão listadas no arquivo `requirements.txt`:

## Endpoints

### `GET /`

Verifica o status da API.

### `GET /items`

Retorna uma lista de itens disponíveis.

### `POST /login`

Gera um token JWT para autenticação.

### `GET /protected`

Acessa uma rota protegida. Requer token JWT.

## Documentação da API

A documentação Swagger está disponível em `http://localhost:1313/swagger`.

## Autenticação

A API usa JWT para autenticação. Para acessar rotas protegidas, inclua o token JWT no cabeçalho da requisição no formato:
