# Go REST API com Clean Architecture

Este é um projeto de exemplo de uma API REST desenvolvida em Go (Golang), utilizando o framework Gin e um banco de dados PostgreSQL. O projeto segue uma estrutura baseada em princípios de Clean Architecture, separando as responsabilidades em camadas: `controller`, `usecase` e `repository`.

## ✨ Features

- **API REST** para operações CRUD de produtos.
- **Framework Gin**: Roteamento e middlewares de alta performance.
- **PostgreSQL**: Banco de dados relacional para persistência de dados.
- **Arquitetura em Camadas**: Organização do código para melhor manutenibilidade e testabilidade.
- **Containerização com Docker**: Ambiente de desenvolvimento e produção consistente e isolado.

## 🛠️ Tecnologias Utilizadas

- Go (v1.23)
- Gin
- PostgreSQL
- Docker & Docker Compose
- lib/pq (Driver do PostgreSQL para Go)

## 🚀 Começando

Para executar este projeto localmente, você precisará ter o Docker e o Docker Compose instalados em sua máquina.

### Pré-requisitos

- Docker
- Docker Compose

### Instalação e Execução

1.  **Clone o repositório:**

    ```bash
    git clone https://github.com/seu-usuario/go-api.git
    cd go-api
    ```

2.  **Inicie os containers com Docker Compose:**

    Este comando irá construir a imagem da aplicação Go e iniciar os containers da aplicação e do banco de dados.

    ```bash
    docker-compose up --build
    ```

3.  **Acesse a aplicação:**

    A API estará disponível em `http://localhost:8000`.

## 📡 Endpoints da API

A seguir estão os endpoints disponíveis atualmente:

| Método | Rota                  | Descrição                                             |
| :----- | :-------------------- | :---------------------------------------------------- |
| `GET`  | `/ping`               | Retorna `{"message": "pong"}` se a API estiver no ar. |
| `GET`  | `/products`           | Lista todos os produtos.                              |
| `POST` | `/product`            | Cria um novo produto.                                 |
| `GET`  | `/product/:productId` | Busca um produto pelo seu ID.                         |

### Próximos Passos

- [ ] Implementar rota `PUT` para atualizar um produto.
- [ ] Implementar rota `DELETE` para remover um produto.
- [ ] Adicionar autenticação JWT para proteger os endpoints.

## 🎓 Créditos e Agradecimentos

Este projeto foi desenvolvido com base no tutorial disponível no YouTube. Um agradecimento especial ao criador do conteúdo por compartilhar seu conhecimento.

> **Nota:** Link do tutorial -> https://www.youtube.com/watch?v=3p4mpId_ZU8
