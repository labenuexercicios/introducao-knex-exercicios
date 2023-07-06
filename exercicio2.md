# Exercício 2

Apague as tabelas SQL de users, products e purchases e as e crie novamente apenas com as colunas descritas abaixo _(são as mesmas colunas que estão nos requisitos finais do projeto)_.

Em seguida, refatore (ou recrie) os seguintes endpoints:

## Create user
Cadastra uma nova pessoa.
```typescript
// Request
// POST /users
// body JSON
{
    "id": "u003",
    "name": "Astrodev",
    "email": "astrodev@email.com",
    "password": "astrodev00"
}

// Response
// status 201 CREATED
{
    message: "Cadastro realizado com sucesso"
}
```

## Create product
Cadastra um novo produto.
```typescript
// Request
// POST /products
// body JSON
{
    "id": "prod003",
    "name": "Teclado gamer",
    "price": 200,
    "description": "Teclado mecânico com numpad",
    "imageUrl": "https://picsum.photos/seed/Teclado%20gamer/400"
}

// Response
// status 201 CREATED
{
    message: "Produto cadastrado com sucesso"
}
```

## Create purchase
Cadastra um novo pedido. Como dica, o exercício 1 da aula de [Relações em SQL II](https://github.com/labenuexercicios/relacoes-sql-II-exercicios) é uma boa referência.
```typescript
// Request
// POST /purchases
// body JSON
{
    "id": "pur001",
    "buyer": "u001",
    "products": [
        {
            "id": "prod001",
            "quantity": 2
        },
        {
            "id": "prod002",
            "quantity": 1
        }
    ]
}

// Response
// status 201 CREATED
{
    message: "Pedido realizado com sucesso"
}
```
    - "Compra cadastrada com sucesso"
