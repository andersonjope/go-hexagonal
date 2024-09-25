# Projeto Go com MockGen e SQLite

Este é um projeto Go que utiliza o `mockgen` para gerar mocks e o SQLite como banco de dados.

## Pré-requisitos

Antes de começar, certifique-se de ter as seguintes ferramentas instaladas:

- [Go](https://golang.org/dl/)
- [SQLite](https://www.sqlite.org/index.html)

### Instalação do SQLite

Para instalar o SQLite, execute o seguinte comando:

```bash
sudo apt-get install sqlite3
```

## Estrutura do Projeto

```plaintext
.
├── application
│   ├── mocks
│   │   └── application.go
│   └── product.go
├── main.go
└── sqlite.db
```

## Gerando Mocks com MockGen

Para gerar os mocks da sua aplicação, use o comando abaixo. Certifique-se de ajustar o caminho do `source` conforme necessário.

```bash
mockgen -destination=application/mocks/application.go -source=application/product.go application
```

## Criando e Inicializando o Banco de Dados

Para criar um banco de dados SQLite e inicializá-lo, execute os seguintes comandos:

```bash
touch sqlite.db
sqlite3 sqlite.db
```

Você pode começar a definir suas tabelas e dados dentro do shell do SQLite.

## Executando a Aplicação

Para rodar sua aplicação, use o comando:

```bash
go run main.go http
```

Certifique-se de que todas as dependências estão instaladas e que o código está compilando sem erros.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para enviar um pull request ou abrir uma issue.

---

Sinta-se à vontade para modificar este README conforme necessário para atender às especificidades do seu projeto!