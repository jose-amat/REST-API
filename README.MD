# API, REST, RESTFUL

#HELLO
- Cliente (Client)
- Garçom (pedidos, levar seus pedidos para a cozinha) (API)
- Cozinha (Server)

## API
API é responsável por estabelecer comunicação entre diferentes serviços (garçom).
- Meio de campo entre as tecnologias
- Intermediador para troca de informações

## REST
Restaurante limpo, que atenda bem, que te dê o que você pede. O REST determina algumas obrigações na transferência de informação.

A transferência de dados é feita geralmente usando protocolo HTTP

O REST delimita algumas obrigações nessas transferências de dados (transferências de resources): 

### Existem 6 NECESSIDADES (Constraints) para ser RESTful

- **_Client-server_** -  Separação do cliente e do servidor, dessa forma poderemos ter uma portabilidade do nosso sistema, por exemplo: usando React para web e React Native para o smartphone.

- **_Stateless_** - Cada requisição que o cliente faz para o servidor, deverá conter todas as informações necessárias para o servidor entender e responder (RESPONSE) a requisição (REQUEST).

- **_Cacheable_** - As respostas para uma requisição deverão de ser explícitas ao dizer se aquela requisição, pode ou não ser _cacheada_ pelo cliente.

- **_Layered System_** - O cliente acessa a uma _endpoint_ sem precisar saber da complexidade que o servidor está lidando para que a requisição (REQUEST) seja respondida (RESPONSE).

- **_Code on demand (optional)_** - Dá a possibilidade da nossa aplicação enviar códigos, como _JavaScript_, e executar no nosso cliente.

## RESTFUL
É a aplicação dos padrões REST.

### Boas Práticas
- Verbos HTTP
  - GET: Receber dados de um Resource.
  - POST: Enviar dados para serem processador por um Resource.
  - PUT: Atualizar dados de um Resource.
  - DELETE: Deletar um Resource.

  ### Status das respostas
  - 1xx: Informação
  - 2xx: Sucesso
    - 200: OK
    - 201: CREATED
    - 204: Não tem conteúdo PUT POST DELETE
  - 3xx: Redirection
  - 4xx: Client Error
    - 400: Bad Request
    - 404: Not Found!
  - 5xx: Server Error 
    - 500: Internal Server Error
