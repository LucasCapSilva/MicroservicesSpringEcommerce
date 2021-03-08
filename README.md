# MicroservicesSpringEcommerce

## executar rabitMQ

 docker-compose up -d
 
 http://localhost:15672/
 
## executar Spring 

http://localhost:8761/registry

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
