### project-avaliation

<br>

# API Node.js Controle de Gastos
<br>
   
![Imagem representativa de controle de gastos](./imagens/img-0.jpg)

<br>    

<p>Muitas pessoas sonham em organizar suas finanças e gastos mensais, mas está cada vez mais difícil alcançar essa meta. Porém, é uma meta perfeitamente alcançável para quem controla a forma como gasta o próprio dinheiro. 
<p>Uma coisa é certa: se você não sabe como controlar seus gastos, não saberá para onde está indo o seu dinheiro. Importante destacar que para você realizar um controle eficiente de gastos será necessário organizar suas finanças pessoais e/ou familiares. Cabe enfatizar ainda que neste processo, por menor que um gasto seja, ele deve ser sempre considerado em seu planejamento financeiro. Então, nada de ignorar aquele cafezinho comprado depois do almoço, só porque custou alguns reais. Nessas horas, todo dinheiro gasto conta.  
</p>
<p>E a pergunta que não quer calar: Você tem educação financeira? </p>
<p>A Educação Financeira não consiste somente em aprender a economizar, cortar gastos, poupar e acumular dinheiro.</p>
<p>É bem mais que isso. É buscar uma melhor qualidade de vida tanto hoje quanto no futuro, proporcionando a segurança material necessária para aproveitar os prazeres da vida e, ao mesmo tempo, ter uma garantia para eventuais imprevistos.</p>

<br>

![Imagem representativa dinheiro siu voando](./imagens/img-1.jpg)

<br>

## Aprenda o básico sobre finanças pessoais :

<br>

### Receitas e Despesas


 - <p>O primeiro passo para cuidar melhor do seu dinheiro é tentar gastar menos do que se ganha, fazer com que as receitas sejam maiores do que as despesas.</p>

 <br>

 ### Juros e inflação

 - <p>Entenda os conceitos de juros e inflação e qual a relação com o seu dia a dia, pois isso ajuda na hora de pegar um empréstimo, escolher um investimento e também na hora de calcular uma conta em atraso.</p>

 <br>

 ### Créditos

 - <p>Os gastos feitos no cartão de crédito precisam ser planejados e a fatura deve ser paga no dia de vencimento, no valor integral, para que seu uso seja vantajoso. Quando as faturas são pagas em atraso, os altos juros cobrados podem transformar o cartão em um vilão do orçamento doméstico.</p>

 <br>

 ### Investimentos

- <p>Investir é, basicamente, emprestar o seu dinheiro ao banco para receber os juros pelo dinheiro emprestado ou aplicar o seu dinheiro em um negócio que vai render lucros.</p>

<br>

### Contas

- <p>​Quando você coloca o seu dinheiro no banco, geralmente você utiliza uma conta bancária para movimentar esses recursos. Como existem diversos tipos de contas (corrente, conjunta, salário, caderneta de poupança, conta universitária, etc.), saber qual é a mais indicada para você dependerá de como você lida com seu dinheiro e qual seu objetivo em ter uma conta.</p>

<br>

<p>Assista abaixo aos vídeos que te darão dicas importantes de como controlar bem seus gastos :
</p>

<br>

[Como controlar meus gastos](https://www.youtube.com/watch?list=PLjyojW8y_HLtabIzCHwE0FFbEVR8qvuPq&v=YyG-bC-8JbA)

<br>

## Descrição da API

<br>

<p>A API Controle de Gastos é uma forma de organizar os gastos de uma determinada pessoa ou dos membros de uma dada família baseada em todas as receitas obtidas e despesas assumidas/realizadas.
O principal objetivo é controlar as entradas e saídas de recursos financeiros do ponto de vista de uma boa e saudável educação financeira.
Na API será possível criar receitas e despesas, bem como exibi-lás, através de alguns endpoints. A manipulação dos dados será realizada através da implementação dos métodos PUT  e DELETE.
Também será implementado um método para mostrar a situação geral da pessoa ou da família com relação ao controle/saúde do orçamento baseado no montante existente no banco de dados .</p>

<br>

## Estrutura do projeto :

<br>

```
├── src
│   ├── controllers
|      ├── despesasController.js
|       ├── receitasController.js
|       ├── transacoesController.js
│   ├── models
|      ├── despesas.js
|      ├── receitas.js
│   ├── routes 
│       ├── despessRoute.js
│       ├── receitasRoute.js
|       ├── transacoesRoute.js
|   ├── app.js
├── package.json
├── server.js
```


<br>

## Tecnologias utilizadas neste projeto :

- Git e GitHub ;
- Node.js ;
- MongoDB ;
- Javascript ;
- Heroku .

<br>

## Funcionalidades da nossa API


<br>

<p>Os protocolos HTTP definem verbos utilizados nas requisições a serem realizadas. Na tabela abaixo, apresentamos alguns verbos e descrevemos suas respectivas funções, bem como as rotas/endpoints específicas a serem chamadas no Postman .</p>

<br>

Verbo   | Descrição                                                | Endpoint   
:---    |:---                                                      |:---            
POST    | Adiciona todas as receitas à sua aplicação               | localhost:3000/receitas
POST    | Adiciona todas as despesas à sua aplicação               | localhost:3000/despesas
GET     | Exibe todas as receitas                                  | localhost:3000/receitas 
GET     | Exibe receitas específicas com base no id                | localhost:3000/receitas/id 
GET     | Exibe todas as despesas                                  | localhost:3000/despesas
GET     | Exibe despesass específicas com base no id               | localhost:3000/despesas/id 
GET     | Exibe a situação financeira atualizada baseado no id     | localhost:3000/transacoes/id 
PUT     | Atualiza ou insere os campos na aplicação (receitas)     | localhost:3000/receitas/id 
PUT     | Atualiza ou insere os campos na aplicação (despesas)     | localhost:3000/despesas/id 
DELETE  | Exclui registros do arquivo de receitas com base no id   | localhost:3000/receitas/id 
DELETE  | Exclui registros do arquivo de despesas com base no id   | localhost:3000/despesas/id 
DELETE  | Exclui registros do arquivo receitas (faturado = false)  | localhost:3000/receitas 
DELETE  | Exclui registros do arquivo despesas (faturado = false)  | localhost:3000/despesas 

<br>

<br>

<p>Para rodar a aplicação é necessário instalar algumas bibliotecas a serem executadas no terminal :</p>

- Express : é o framework Node e a biblioteca subjacente para uma série de outros frameworks do Node, sendo instalada através do comando npm install express --save  ; 
- Nodemon : esse módulo é uma ferramenta que ajuda a desenvolver aplicativos baseados em node.js que irá monitorar todas as alterações nos arquivos da sua aplicação e reiniciar automaticamente o servidor quando for necessário e sendo executado através do comando npm install nodemon .
- Mongoose :  é uma ferramenta de modelagem de objetos MongoDB projetada para funcionar em um ambiente assíncrono, oferecendo suporte a promessas e retornos de chamada; devendo ser instalada através do comando npm install mongoose --save .

<br>

## Referências:  

<br>

https://www.caixa.gov.br/educacao-financeira

https://mongoosejs.com/docs/

https://www.npmjs.com/package/nodemon

 