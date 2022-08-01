String com número é concatenação.

var so se usa uma única vez, declaro apenas uma vez no meu sistema

function é verbo de ação, pra deixar claro o que ela faz.
função guarda um chamada que posso usar durante o código.

Toda função tem uma ou mais funções.



# Como a função prompt sempre retorna o que digitamos no formato 
texto, ou seja, como um string, é uma boa prática sempre convertermos o valor digitado para número quando nossa intenção é ler um número. Vamos analisar esta instrução:

{
    var convidados = parseInt(prompt("Número de convidados"))
}
A função prompt retorna o que digitamos como string e esse retorno é passado para parseInt. É esta função que recebe uma string e a converte para número. Agora, como temos dois números ligados, não acontecerá mais a concatenação, mas sim a soma.


# Sabemos que operações lógicas podem resultar em true (verdadeiro) ou false (falso). Sendo assim, temos as seguintes operações:

a) 1 == 1
b) 10 < 11
c) 1 >= 1
d) 2 <= 1
e) 9 > 8

a) true
b) true
c) true
d) false
e) true

Vejamos cada operação:

a) 1 == 1 é true, porque 1 é igual a 1.

b) 10 < 11 é true, porque 10 é menor que 11.

c) 1 >= 1 é true, porque 1 é maior ou igual a 1.

d) 2 <= 1 é false, porque 2 não é menor ou igual a 1.

e) 9 > 8 é true, porque 9 é maior que 8.

--------------------------------------------------------------------

# Qual das opções abaixo usa corretamente a condição if e else ?

Alternativa correta
var senha = prompt("Entre com sua senha");

if(senha == "calopsitaazul") {

    alert("Acesso liberado!");
} else {

    alert("Acesso negado!");
}

A condição if precisa receber o resultado de uma operação lógica dentro de seu parênteses.

var senha = prompt("Entre com sua senha");

if(senha == "calopsitaazul")

Além disso, é dentro do seu bloco que indicamos qual ou quais instruções serão executadas se a operação lógica der true:

var senha = prompt("Entre com sua senha");

if(senha == "calopsitaazul") {
    alert("Acesso liberado!");    
}

Veja que temos as duas chaves que iniciam e terminam o bloco if. A instrução else vem logo após o fechamento do bloco if:

var senha = prompt("Entre com sua senha");

if(senha == "calopsitaazul") {
    alert("Acesso liberado!");    
} else

Assim como a instrução if, a else também possui seu bloco com as instruções que desejamos executar se a condição if receber false:

var senha = prompt("Entre com sua senha");

if(senha == "calopsitaazul") {

    alert("Acesso liberado!");
} else {

    alert("Acesso negado!");
}