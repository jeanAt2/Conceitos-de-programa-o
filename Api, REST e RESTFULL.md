Entende uma parte do contexto de backend;

### API

Cliente (Client)

Garço ( Pedido, levar os seus pedidos, para a cozinha) - Nossa API

Cozinha (Server);

É uma conversa entre o seu APP com o servidor;

### REST

Acrônimo para REpresentational State Transfer (Transferencia de Estado Representativo);

São regras na troca dessas informções

Usando o protocolo HTTP;

Resources é uma entidade um objeto;

### 6 NECESSIDADES (constrains) para ser RESTFull

- _Client-server_: Eles precisam estar separados.
- Client React, ReactNative são exemplos de clientes;
  Server: Nosso backend é o que sustenta a aplicação, guardando todas as informações que são consultadas pelo nosso cliente. Podendo ser feito por diversar linguagens com java, javascript,php e outras.

- _Stateless_: (Sem estado) Cada requisição que o Cliente faz para o servidor, devera conter todas as informações necessárias para o servidor entender e responder(RESPONSE) a requisição(REQUEST). Exemplo A sessão do usuário deverá ser enviada em todas as requisições, para saber se aquel usuário está autenticado e apto a usar os serviços, e o servidor não pode lembrar que o cliente foi autenticado na requisição anterior.

- _Cacheable_: AS respostas para uma requisição deverá apresentar se o cliente pode ou não ser cacheado pelo cliente.

- _Layerd System_: Sistemas de camadas

### RESTFULL

RESTfull, é a aplicação dos padrões REST.
