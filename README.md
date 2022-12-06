# Desafios

## Desafio 1

Desenvolva um sistema para a biblioteca da UTFPR. Em conversa com o funcionário 
responsável por manter a organização dos livros, ele lhe informou que cada livro possui título, 
autor, editora, número total de páginas e ano de publicação. Todas as características do livro 
devem ser inicializadas no momento da criação do mesmo. Além disso, o sistema deve 
permitir que um livro seja emprestado. Para isso, deve-se saber o nome do aluno que está 
efetuando o empréstimo. Só será permitido realizar o empréstimo se o livro estiver disponível 
no momento, ou seja, não estiver sido emprestado. Ao emprestar um livro, deve-se armazenar 
o nome do aluno que realizou o empréstimo. Além dessa funcionalidade, deve ser possível 
devolver um livro emprestado. Para isso, é necessário saber quantos dias o aluno ficou com 
o livro. A devolução ocorrerá se o livro estiver realmente emprestado. Se o empréstimo 
extrapolou o número de 7 dias, deverá ser calculado o valor da multa, a qual corresponde a 3 
reais por dia de atraso. Ao realizar a devolução, deverá ser informado ao usuário que o livro 
foi devolvido com sucesso e, se houver multa, qual o valor que deverá ser pago por ele. Uma 
vez que o livro foi devolvido, será permitido ser emprestado novamente a outro aluno. 
Uma vez definidos os dados do livro na sua criação, os mesmos não poderão ser alterados 
por classes externas. Por fim, declare o método toString( ), que retornará a concatenação de 
todos os valores pertinente ao livro em uma espécie de “relatório” do objeto, este deve conter 
se o livro está ou não emprestado e, se sim, qual o nome do aluno que o emprestou. 
Para realizar a instanciação dos livros, bem como executar suas funcionalidades, crie uma 
classe de testes.


## Desafio 2

Uma empresa de cartões de créditos contratou você para desenvolver o sistema do mais novo 
programa de pontuação aos clientes que possuem boa reputação. Em uma conversa com o 
diretor desta empresa ele lhe explicou que possuem dois cartões: cartão de crédito comum e 
cartão de crédito premium. 
O cartão de crédito comum é identificado por um número de identificação, senha (numérica), 
nome do titular, valor do limite, valor da fatura. Sendo que todas as características do cartão 
comum devem ser inicializadas no momento da criação do mesmo, porém o valor da fatura, 
obrigatoriamente, deve ser iniciado com valor 0,00 (zero), pois o cliente ainda não efetuou 
nenhum compra. O diretor da empresa ainda comentou que com o cartão de crédito comum 
deve ser possível bloquear e desbloquear o cartão, visualizar a fatura e fazer compra. Para 
realizar o bloqueio do cartão é necessário saber a senha do mesmo, uma vez verificada se a 
senha está correta, o cartão pode então ser bloqueado. O desbloqueio do cartão segue o 
mesmo princípio, deve-se receber a senha, se a mesma estiver correta, o cartão é 
desbloqueado. Para realizar a visualização da fatura, primeiramente deve-se receber a senha 
do cartão e verificar se esta está correta. Uma vez confirmada essa informação, deve-se exibir 
o nome do cliente atrelado ao cartão, valor da fatura e o valor do limite disponível. Por fim, 
para fazer a compra de produtos é necessário saber qual produto está sendo adquirido e a 
senha do cartão. Um produto é caracterizado por uma data da compra, nome do produto e 
valor do produto (em reais). Para realizar a compra, é necessário que: (i) o cartão esteja 
desbloqueado; (ii) a senha esteja correta; e (iii) o valor do produto seja menor ou igual ao valor 
do limite do cartão. Se todas as condições forem satisfeitas, a compra poderá ser realizada, 
ou seja, o valor do produto que está sendo comprado seve ser somado ao valor da fatura, e 
o valor do produto deve ser subtraído do valor do limite. Além disso, deve-se mostrar uma 
mensagem de confirmação ao usuário contendo os dados do Produto (data da compra, nome 
do produto e valor do produto (em reais)). Caso alguma dessas condições não forem 
satisfeitas, deve-se exibir ao cliente a mensagem respectiva do erro. Ex.: “cartão bloqueado”,
“senha incorreta” ou “limite insuficiente”. Obs.: na última página há uma explicação como 
funciona o valor do limite do cartão de crédito comum e valor da fatura.
O cartão de crédito premium é identificado pelo seu número de identificação, senha 
(numérica), nome do titular, valor da fatura e pontuação. Todas as características devem ser 
inicializadas no momento da criação do mesmo, porém, o valor da fatura e a pontuação 
devem, obrigatoriamente, ser inicializados com valor 0 (zero), visto que o cartão ainda não foi 
utilizado. Além disso, deve ser possível bloquear e desbloquear o cartão, visualizar a fatura e 
fazer compra. Para realizar o bloqueio, é necessário receber a senha do cartão e, após 
verificar se a mesma está correta, o bloqueio pode ser realizado. O desbloqueio é semelhante, 
é necessário receber a senha e o desbloqueio só deve ocorrer após a verificação da mesma. 
Para visualizar da fatura, é necessário receber a senha do cartão, se essa estiver correta, 
então será mostrado o nome do cliente, valor da fatura e a pontuação. Por fim, para fazer a 
compra é necessário saber qual produto deseja comprar e a senha do cartão de crédito. A 
compra só deve ser realizada se o cartão não estiver bloqueado e se a senha estiver correta. 
Caso ambas as condições forem satisfeitas, deve ser exibido a confirmação da compra 
contendo os dados do produto (data da compra, nome do produto e valor do produto (em 
reais)). Além disso, o valor do produto que está sendo comprado deve ser somado ao valor
da fatura. Então será realizado o cálculo da pontuação. A fórmula para realizar o cálculo da 
pontuação é dada por: Para cada 1 dólar (US$) gasto, equivale à 1 ponto. Considere que o 
dólar equivale a R$5,00. Ou seja, um produto que custa R$100,00, equivale a US$20,00, logo, 
esse produto gera 20 pontos.
Para realizar a instanciação dos objetos, bem como executar suas funcionalidades, crie uma 
classe de testes.

### - Valor de Limite

Imagine o seguinte cenário: o cartão de crédito comum possui um limite de R$1000,00. Você 
então realiza um compra do Produto A, que custa R$700,00. Após realizar a compra, seu 
limite, que era de R$1000,00, agora é de R$300,00 (1000,00 – 700,00). Você então realiza a 
compra do Produto B, que custa R$250,00. Após realizar a compra, seu limite agora é de 
R$50,00. O valor do Produto a ser adquirido não pode ultrapassar o valor do limite. Neste 
caso, você não poderá comprar outro produto que ultrapasse seu limite atual (R$50,00).
Semelhante a uma conta poupança na qual você não pode gastar mais do valor que tem em 
sua conta.

### - Valor da Fatura

Imagine o seguinte cenário: o cartão de crédito é recém adquirido, consequentemente, o valor 
da fatura é R$0,00 (zero), pois ainda não foram adquiridos nenhum produto. Ao realizar a 
compra de um PRODUTO Z de R$250,00, esse valor será somado ao valor da fatura (250,00 + 0,00), então o valor da fatura agora será de R$250,00. A realizar uma compra do Produto Y 
que custa de R$100,00, a fatura passará a ser R$350,00 (100,00 + 250,00). E assim 
sucessivamente, como uma espécie de extrato de conta corrente


## Desafio 3

Você foi contratado para desenvolver um sistema para uma locadora de veículos. Em uma 
conversa com o gerente desta locadora ele lhe explicou que o sistema da locadora deve ser 
capaz de armazenar os 4 veículos que ela contém. Além dos veículos, a locadora é 
identificada pela sua razão social (nome) e cnpj. Todos os atributos devem ser inicializados 
no momento da criação do objeto. Sendo a razão social e o cpnj recebidos por parâmetros
e os veículos da locadora podem ser definidos estaticamente no momento da 
instanciação do vetor, não sendo necessário recebe-los por parâmetro. Além disso, a
própria locadora deve ser responsável por controlar a locação e devolução de cada veículo, 
além de ser possível consultar os dados de todos os veículos. Sabe-se que cada veículo é 
identificado pelo seu modelo, marca, placa e valor da diária que é cobrada em cada dia que 
o veículo permanece locado. Para a realização da locação de um veículo, é necessário saber 
a placa, nome do cliente que deseja locar o veículo, dia da locação e dia previsto para 
devolução. O sistema deve ser capaz de buscar o veículo que contém aquela placa e se o 
mesmo estiver disponível para locação, a locação poderá ser realizada. Ainda na locação, o
funcionário lhe explicou que é importante armazenar o dia que ocorreu a locação, dia previsto 
para a devolução e o nome do cliente, pois esses dados são importantes em outras 
funcionalidades do sistema. Obs.: a fim de facilitar o exercício, adote apenas o dia, 
desconsiderando meses e anos. Para realizar a devolução do veículo, é necessário saber 
a placa do veículo que está sendo devolvido e o dia que está ocorrendo a devolução. O 
sistema deve buscar qual é o veículo que possui aquela placa e se o mesmo estiver realmente 
locado, poderá realizar a devolução. Para isso, deverá ser calculado o valor total da locação. 
O cálculo considera se o veículo foi entregue até o dia previsto, se sim, então é realizado um 
cálculo de multiplicação considerando o número de dias que o veículo permaneceu locado e 
o valor da diária daquele veículo. Caso o veículo foi entregue com atraso, ou seja, em um dia 
além do que estava previsto, será cobrado, além do valor normal em relação aos dias previstos, o valor dobrado da diária em cada dia de atraso. Exemplo: se o veículo possui 
diária de R$ 100,00, foi locado no dia 5 com dia de entrega previsto para dia 8 e o cliente 
devolveu no dia 8, então será cobrado R$300,00 (valor da diária * quantidade de dias). 
Porém, se o cliente realizou a devolução dia 10, ou seja, com 2 dias de atraso, esses 2 
dias serão cobrados o valor da diária dobrados, além dos valores normais entre os dias 
5 e 8. O valor total neste cenário é de R$ 700,00 (R$ 300,00 entre os dias 5 e 8, R$ 400,00 
entre os dias 9 e 10 que está em atraso). Por fim, o sistema deve possibilitar que seja exibido 
todos os dados de todos os veículos contidos na locadora, inclusive se o veículo está ou não 
locado, e, se sim, deve-se exibir o dia que o mesmo foi locado, dia previsto para a devolução 
e o nome do cliente que o locou.


