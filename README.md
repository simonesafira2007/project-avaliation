# project-avaliation

### api_controle_de_gastos
<br>

## API Node.js Controle de Gastos
<br>
   
![Imagem representativa de controle de gastos](./imagens/img-0.jpg)

<br>    

<p>Muitas pessoas sonham em organizar suas finanças e gastos mensais, mas está cada vez mais difícil alcançar essa meta. Porém, é uma meta perfeitamente alcançável para quem controla a forma como gasta o próprio dinheiro. 
<p>Uma coisa é certa: se você não sabe como controlar seus gastos, não saberá para onde está indo o seu dinheiro. Importante destacar que para você realizar um controle eficiente de gastos será necessário organizar suas finanças pessoais e/ou familiares. Cabe enfatizar ainda que neste processo, por menor que um gasto seja, ele deve ser sempre considerado em seu planejamento financeiro. Então, nada de ignorar aquele cafezinho comprada depois do almoço, só porque custou alguns reais. Nessas horas, todo dinheiro gasto conta.  
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
Também será implementado um código para mostrar a situação da pessoa ou da família em relação ao controle do orçamento.</p>
<p>Protocolos HTTP definem os verbos utilizados nas requisições, bem como suas respectivas funções e rotas específicas a serem chamadas no navegador ou no Postman</p>



Verbo   | Descrição                                                | Endpoint   
:---    |:---                                                      |:---            
POST    | Adiciona todas as receitas à sua aplicação               |localhost:3000/receitas
POST    | Adiciona todas as despesas à sua aplicação               |localhost:3000/despesas
GET     | Exibe suas receitas atualizadas                          |localhost:3000/receitas 
GET     | Exibe receitas específicas com base no id                |localhost:3000/receitas/id 
GET     | Exibe sua despesas atualizadas                           |localhost:3000/despesas
GET     | Exibe despesass específicas com base no id               |localhost:3000/despesas/id 
GET     | Exibe a situação financeira atualizada                   |localhost:3000/transacoes [wip]
PUT     | Atualiza ou insere os campos na aplicação (receitas)      | localhost:3000/receitas/id
PUT     | Atualiza ou insere os campos na aplicação (despesas)      | localhost:3000/despesas/id
DELETE  | Exclui registros do arquivo de receitas com base no id    | localhost:3000/receitas/id
DELETE  | Exclui registros do arquivo de despesas com base no id    | localhost:3000/despesas/id
DELETE  | Exclui registros do arquivo receitas (faturado = false)   | localhost:3000/receitas
DELETE  | Exclui registros do arquivo despesas (faturado = false)   | localhost:3000/despesas

<br>

## Referências:

<br>

https://www.caixa.gov.br/educacao-financeira
