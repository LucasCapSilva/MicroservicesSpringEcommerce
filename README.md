# MicroservicesSpringEcommerce

## Executar os microservicos

 ![alt text](https://i.imgur.com/i52vFnQ.png)
 
 

## executar rabitMQ

 docker-compose up -d
 
 http://localhost:15672/
 
 user: admin
 password: admin
 
 ## add filas
 
 crud.produto.queue
 
 ![alt text](https://i.imgur.com/quRI7V2.png)
 
## Criar uma nova instancia

 ![alt text](https://i.imgur.com/l4NlyQs.png)


## executar Spring Eureka

http://localhost:8761/registry

 ![alt text](https://i.imgur.com/dCPsf1B.png)
 
 

## login 

http://localhost:8080/api/auth/login POST

{
    "userName":"lucas@email.com",
    "password":"123456"
}

## Cadastro produto

http://localhost:8080/api/crud/produto POST
{
    "nome":"Celular",
    "estoque":"50",
    "preco":"80.00"
}

## Cadastro de venda

http://localhost:8080/api/pagamento/venda/ POST

{
                "data": "2020-10-07T00:00:00.000+00:00",
                "produtos": [
                    {
                        "idProduto":1,
                        "quantidade":1
                    }
                ],
                "valorTotal": 2000.0
               
}

## mostrar endPorta loadBalance

http://localhost:8080/api/pagamento/venda/mostrarPorta


 ![alt text](https://i.imgur.com/IZ0Dmvl.png)


