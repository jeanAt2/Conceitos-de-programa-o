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

- _Layerd System_: Sistemas em camadas exemplo "https://localhost/user";
  O Cliente acessa o endpoint, sem precisar saber da complexidade, de quais passos estão sendo necessários para o servidor responder a requisição, ou quais requisição seja respondida.

- _Code on demand (Opitional)_: Dá a possibilidade da nossa aplicação pegar códigos, como o javascript, por exemplo e executar no cliente.

### RESTFULL

RESTfull, é a aplicação dos padrões REST.

### Criando a API

yarn init -y(Para não precisar preencher os campos de inicio do projeto)
ou
npm init -y

- Podemos adicionar a biblioteca EXPRESS para criar a noss API

yarn add express
ou
npm -i express

Vá no repositório Projetos-init para ver o código de criação da API;

Temos que entender bem um conceito que é o resouce.

### Resouce

É um objeto, uma entedidade com uma ou vários relacionamentos com outros resoucers. Vamos farlar sobre "verbos HTTP".

### VERBOS HTTP.

(Há mais, porem esses são os principais);

- GET: recebe dados de um Resouce
- POST: Envia dados ou informações para serem processados por um resouce.
- PUT: Atualizar os dados de um resouce;
- DELETE: Vai deletar os dados de um resouce

_clients_ - é o nosso endPoint e o nome do nosso resouce

http://localhost:3000/_clients_

nop express é facil de se usar os verbos http

app.get();
app.post();
app.put();
app.delete();

# STATUS DE REPOSTAS

- 1xx: Informação
- 2xx: Sucesso
- 200: OK
- 201: CREATED
- 204: Não tem conteúdo PUT POST DELETE
- 3xx: Redirection
- 4xx: Client Error
- 400: Bad Request
- 404: Not Found!
- 5xx: Server Error 500: Internal Server Error

# Boas praticas

- Utilizar verbos HTTP para nossa requisições
- Utilizar plural ou singular na criação dos endpoints? _Não importa_ use um padrão.
- Não deixar barra no final do endpoints.
- Nunca deixe o cliente sem reposta.
