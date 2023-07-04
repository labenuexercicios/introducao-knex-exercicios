# Exerício 1
A partir de agora, vamos abandonar o uso do arquivo database.ts!
Configure seu servidor Express para que ele se comunique com seu banco de dados (arquivo .db) via knex e refatore (ou recrie) os seguintes endpoints:

## Get All Users
- method HTTP (GET)
- path ("/users")
- response
    - status 200
    - array de users do arquivo .db
 
-------------

## Get All Products
- method HTTP (GET)
- path ("/products")
- response
    - status 200
    - array de products do arquivo .db
      
----------------

## Get all products - funcionalidade 1

##### Nessa funcionalidade, NÃO devemos criar um novo endpoint para o Get All Products, é nescessário apenas adicionar essa funcionalidade ao enpoint

- method HTTP (GET)
- path ("/products")
- query params
    - name (exemplo de como deve ficar todo o caminho /products?name=gamer )
- response
    - status 200
    - array do resultado da busca no arquivo .db
