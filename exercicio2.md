# Exercício 2

Apague as tabelas SQL de users, products e purchases e as e crie novamente apenas com as colunas descritas abaixo _(são as mesmas colunas que estão nos requisitos finais do projeto)_.

Em seguida, refatore (ou recrie) os seguintes endpoints:

## Create User
- method HTTP (POST)
- path ("/users")
- body
    - id
    - name
    - email
    - password
    - createdAt
- response
    - status 201
    - "Cadastro realizado com sucesso"

## Create Product
- method HTTP (POST)
- path ("/products")
- body
    - id
    - name
    - price
    - description
    - imageUrl
- response
    - status 201
    - "Produto cadastrado com sucesso"

## Create Purchase
- method HTTP (POST)
- path ("/purchases")
- body
    - id
    - buyer
    - totalPrice
    - createdAt

    
- response
    - status 201
    - "Compra cadastrada com sucesso"
