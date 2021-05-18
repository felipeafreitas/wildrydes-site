
# wildrydes

A rebuild of the serverless website WildRydes Workshop in Vue.js with AWS Amplify CLI.

[Clique aqui para acessar o projeto final](https://main.dfrg7cickqo1u.amplifyapp.com/)

**Esse projeto foi feito como parte do processo seletivo do Nexo Jornal.**
 
 
 ## Day 0: Escolha do Projeto
**Trilha escolhida:** [Crie uma aplicação Web sem servidor](https://aws.amazon.com/pt/getting-started/hands-on/build-serverless-web-app-lambda-apigateway-s3-dynamodb-cognito/)

Nas minhas experiências recentes, tenho com frequência desenvolvido e participado de projetos me voltando ao front-end. Soma-se a isso o fato de que nunca tive um contato direto com os recursos da AWS.

Como se trata de uma vaga para full stack, entendi que percorrer esse tutorial seria uma boa forma de desenvolver outros conceitos e habilidade, e me preparar para a oportunidade de uma forma mais completa. 

Atualmente, trabalho como desenvolvedor front-end, utilizando principalmente as tecnologias React e React Native.

Nesse documento, pretendo registrar com comentários e printscreens o meu percurso nesse tutorial.

**Sobre o projeto:** Se trata da implementação de uma aplicação utilizando os serviços da AWS para configurar o backend Serveless. A aplicação é um "Uber de Unicórnios"



## Day 1: Hospedar um site Estático
Ferramenta utilizada: AWS Amplify

Antes, eu havia utilizado o Netlify e o próprio github pages para deploy do front-ent.
Primeiro passo: conta na AWS, criação do repositório, configuração do ambiente.

Primeiro problema enfrentado: não tenho configurado o CLI da AWS. E infelizmente, o tutorial não especifica muito bem como seguir quais passos seguir nesse sentido.

Minha solução foi buscar tutoriais auxiliares:

-   [](https://webapp.serverlessworkshops.io/staticwebhosting/repository/)[https://webapp.serverlessworkshops.io/staticwebhosting/repository/](https://webapp.serverlessworkshops.io/staticwebhosting/repository/)
-   [](https://github.com/aws-samples/aws-serverless-workshops/tree/master/WebApplication)[https://webapp.serverlessworkshops.io/setup/](https://webapp.serverlessworkshops.io/setup/)

Mensagens de erro no terminal, que diz que eu não tenho as credenciais. 

### Printscreens:

1. Processo de Deploy do Site Estático na AWS Amplify
![Processo de Deploy do Site Estático na AWS Amplify](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/6a4fffcc-c84d-46cc-8234-7a1fd567c5f0/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5/20210518/us-west-2/s3/aws4_request&X-Amz-Date=20210518T215212Z&X-Amz-Expires=86400&X-Amz-Signature=c208c61f760851fa029caa6a5a01888c6a752d6d5074d46e8ee1427c17533123&X-Amz-SignedHeaders=host&response-content-disposition=filename%20=%22Untitled.png%22)

2. Configuração do ambiente de Deploy
![enter image description here](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/f483ffee-c97a-46a8-a798-7972ae85c9e4/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5/20210518/us-west-2/s3/aws4_request&X-Amz-Date=20210518T215225Z&X-Amz-Expires=86400&X-Amz-Signature=447e4ccec16677af860de5936675fda2fe034f0b774241c0c69aefd57859bb5d&X-Amz-SignedHeaders=host&response-content-disposition=filename%20=%22Untitled.png%22)

3. Deploy feito com Sucesso
![enter image description here](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/3670ab5a-eccf-491b-a231-569c68e3c898/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5/20210518/us-west-2/s3/aws4_request&X-Amz-Date=20210518T215253Z&X-Amz-Expires=86400&X-Amz-Signature=b99e34b286371aa716f5c57fe4267aefa93abbe2bc383eba56abda9cf16171e0&X-Amz-SignedHeaders=host&response-content-disposition=filename%20=%22Untitled.png%22)

## Day 2: Gerenciamento de Usuários
Serviço utilizado: Amazon Cognito

Novamente, enfrentei alguns problemas co o tutorial original aqui. Por isso, acabei de guiando principalmente pela outra versão que encontrei.

Tive que instalar o CLI da AWS

### Printscreens
1. Configurando o ambiente CLI do ampify no meu terminal
![enter image description here](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/3745c91b-919e-45d0-a670-1529bb020eb8/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5/20210518/us-west-2/s3/aws4_request&X-Amz-Date=20210518T215412Z&X-Amz-Expires=86400&X-Amz-Signature=b048a3ef6b6d0530441766d948b3ddd78a2e4d86e83bd0d694e363a18ab0ed3d&X-Amz-SignedHeaders=host&response-content-disposition=filename%20=%22Untitled.png%22)

2. Teste do processo se Cadastro no Site
![enter image description here](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/651e9dec-7b3d-4da1-adbf-a464444ba122/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5/20210518/us-west-2/s3/aws4_request&X-Amz-Date=20210518T215428Z&X-Amz-Expires=86400&X-Amz-Signature=592210544ae621d46b6d770412c021175d1afe30f67d95dbf667ae34aa66652d&X-Amz-SignedHeaders=host&response-content-disposition=filename%20=%22Untitled.png%22)

3. Página Login Feito com Sucesso
![enter image description here](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/ab6a08c1-993e-4396-bb61-da6b54c46df8/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5/20210518/us-west-2/s3/aws4_request&X-Amz-Date=20210518T215458Z&X-Amz-Expires=86400&X-Amz-Signature=958287d26680c513f7d56f2bc2a22d464122671db9e7fb2419dfde2ed0f31f7c&X-Amz-SignedHeaders=host&response-content-disposition=filename%20=%22Untitled.png%22)

## Day 3: Serveless Backend

À partir dessa etapa, todo o processo se deu de forma bem tranquila. A maior parte do trabalho foi feita no ambiente da AWS, acessando a página dos produtos e os configurando. 

Nessa etapa, utilizei as ferramentas AWS Lambda e Amazon DynamoDB para configurar o ambiente de Backend Serveless da aplicação.

Primeiro, foi configurada uma nova tabela no DynamoDB para armazenar as corridas do App. Após isso, foi criada uma função Lambda através do AWS Lambda Console, em que foi implementado um código pronto.

### Printscreens

1. Implementação da Função Lambda
![enter image description here](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/62aa4e16-bb97-4355-8a08-6f70d9b3c14e/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5/20210518/us-west-2/s3/aws4_request&X-Amz-Date=20210518T215609Z&X-Amz-Expires=86400&X-Amz-Signature=20b6339e665544d527d1638352f3959fb4d4923de7be8e82c3be88efa46a4aca&X-Amz-SignedHeaders=host&response-content-disposition=filename%20=%22Untitled.png%22)

2. Criação do teste da função Lambda
![enter image description here](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/c5213959-dc0c-4af8-82cc-82991ed7f39b/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5/20210518/us-west-2/s3/aws4_request&X-Amz-Date=20210518T215529Z&X-Amz-Expires=86400&X-Amz-Signature=7d17b43ca43b0ab1abc1debf8d52d885a735c2a8e10c4962ce3ae182c5cb171f&X-Amz-SignedHeaders=host&response-content-disposition=filename%20=%22Untitled.png%22)

3. Mensagem de sucesso da função Lambda
![enter image description here](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/234c26e1-92d9-4734-8a0c-bfb885390c8f/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5/20210518/us-west-2/s3/aws4_request&X-Amz-Date=20210518T215555Z&X-Amz-Expires=86400&X-Amz-Signature=cbfb212363778f00eb67ddb1e82ae0ee45c0c9800923efcca965c3a281bf37d5&X-Amz-SignedHeaders=host&response-content-disposition=filename%20=%22Untitled.png%22)



## Day 4: Restful API

Por fim, o tutorial me levou a criação de uma Restful API que permita realizar as requisiçoes da aplicação (no caso, o pedido de carona de um unicórnio). A ferramenta utilizada o Amazon API Gateway Console

Essa parte em específica achei extremamente interessante. Ao fim de um bootcamp que recentemente terminei pela Ironhack, havia desenvolvido uma aplicação de e-commerce fullstack, em que desenvolvi uma Rest API utilizando NodeJS, Express e MongoDB. Utilizar o serviço da AWS me impressionou muito, tanto pela nova forma de se realizar quanto pela incrível facilidade do processo. 

A tela para fazer o "pedido" da carona pode ser acessada através desse [link](https://main.dfrg7cickqo1u.amplifyapp.com/ride)

### Printscreens

1. Criação de uma API Restful
![enter image description here](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/2beaa529-c9e0-4fb1-aeb7-55e1f8089eb0/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5/20210518/us-west-2/s3/aws4_request&X-Amz-Date=20210518T215702Z&X-Amz-Expires=86400&X-Amz-Signature=2135bf9adeb1a9c98cf7189ca8ae92849ffc11eab2058ab69aa52f3f15219534&X-Amz-SignedHeaders=host&response-content-disposition=filename%20=%22Untitled.png%22)

2. Mesagem de sucesso do tedte de Integração da API Recém criada com o App
![enter image description here](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/786c553f-4cca-4702-b750-860f8def8787/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5/20210518/us-west-2/s3/aws4_request&X-Amz-Date=20210518T215647Z&X-Amz-Expires=86400&X-Amz-Signature=e038aeadb8d4aeb0502e5da0b916920ea80f2057e3637925c588d89a5c996536&X-Amz-SignedHeaders=host&response-content-disposition=filename%20=%22Untitled.png%22)

3. Execução da Aplicação: Clicar em algum lugar do mapa e pedir um unicórnio com sucesso
![enter image description here](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/2815006a-e343-4abf-adbb-221533c24b12/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5/20210518/us-west-2/s3/aws4_request&X-Amz-Date=20210518T215722Z&X-Amz-Expires=86400&X-Amz-Signature=76e7ceb4197eb75c3927015ddb43bddf4fb36d50dff8a43e445cf5f91b79cb7a&X-Amz-SignedHeaders=host&response-content-disposition=filename%20=%22Untitled.png%22)
