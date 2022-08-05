while {
    estrutura de repetição

# Lembre-se que while repetirá TODAS as instruções que estiverem dentro do seu bloco e a condição passada para ele for true. Veja que while recebe em seus parênteses () a expressão contador <= 10.

Aprendemos que expressões como essa retornam true ou false. Sendo assim, quando no navegador interpretar a linha do while perguntará: o valor da variável contador é menor que ou igual a 10? Como a variável contador recebeu o valor 1 em sua inicialização o resultado da expressão contador <= 10 será true. Sendo assim, o while terá autorização para executar a instrução dentro do seu bloco, no caso, a instrução mostra("Você errou"); e a instrução contador = contador + 1.

Faz sentido ele executar mostra("Já era, você errou!");, claro, mas você lembra a razão de fazermos contador = contador + 1? Veja que essa variável só existe por causa de uma finalidade: é ela que quebrará o lanço de repetição do while. A cada repetição do mostra, precisamos incrementá-la para saber que já mostramos, uma, duas, três vezes e por ai vai. Se não tivermos a instrução contador = contador + 1 nunca a condição passada para o while dará false e cairemos em uma repetição infinita, o famoso loop infinito.
}

# Sabendo que a função (isNaN) recebe um parâmetro e retorna true caso o parâmetro passado seja NaN, qual das opções abaixo  altera corretamente o código de Daniel para usar a função isNaN?

        var idade = parseInt(prompt("Digite sua idade."));
  
        while(isNaN(idade) == true) {
            idade = parseInt(prompt("Digite sua idade."));
        }
        alert(idade);

# Eles precisam convertê-lo de maneira a usar a instrução for

    var contador = 1;
    while(contador <= 10) {
    alert("Contador atual: " + contador);
    contador = contador + 1;
    }

    for(var contador = 1; contador <= 10; contador++) {
        alert("Contador atual: " + contador);
    }

# (Var totalIdade = 0); fora do loop do while; para poder acumular, não se pode ser dentro do laço.
    var totalFamiliares = parseInt(prompt("Quantidades de familiares?"));
    var numero = 1;
    var totalIdades = 0;
    while (numero <= totalFamiliares) {
        var idade = parseInt(prompt("Informe a idade do familiar"));
        totalIdades = totalIdades + idade;
        numero++
    }


# Para saber mais: parseFloat e quando usar?
var numero = parseInt("12.13");
var numero = parseFloat("12.13");

# O primeiro for cria as linhas.
    // O segundo laço for, faz a repetição das estrelinhas em cada linha;
    for(var linha = 1; linha <= 3; linha++) {
        
        for(var coluna = 1; coluna <= 10; coluna++) {
            document.write("*");
        }
        pulaLinha();
    }
#  ------------------------------------------------------------ #

         DIFERENTE !=
        // Math.random - Me gera números aleatórios. 
        // Match.round - Arredonda os números.
        // Match.round(Math.random() * 10);

#  ------------------------------------------------------------ #


<meta charset="UTF-8">

<input />
<button>Clique-me</button>

<script>
    var entrada = document.querySelector("input");
    var botao = document.querySelector("button");
</script>

Você aprendeu que através de document.write escrevemos na tela, mas o document sabe fazer mais coisas. É através de document.querySelector que podemos ir lá no mundo HTML e trazer o elemento para o mundo JavaScript para que possamos manipulá-lo. Mas cuidado, o correto é querySelector com S maiúsculo. Se por acaso você escrever com 's' minúsculo cometerá um erro de sintaxe.

Continuando... O document.querySelector recebe um parâmetro o nome da tag que desejamos buscar do mundo HTML. Ele é mais poderoso do que você imagina e aceita receber outros tipos de parâmetros, mas para nosso treinamento, entender que se passarmos o nome de uma tag HTML ele nos devolverá a tag no mundo JavaScript é suficiente. Há outros jargões envolvidos nesse processo, mas não se preocupe. Você saberá todos eles se quiser continuar seus estudos na linguagem JavaScript.

# Dando tchau no clique de um botão
<meta charset="UTF-8">

<button>Clique-me</button>

<script>
    function tchau() {

        alert("Tchau!!!!!")
    }

    var button = document.querySelector("button");
    button.onclick = tchau;

</script>

# Aprendemos que é através de document.querySelector que buscamos um elemento (TAG) no mundo HTML e o trazemos para o mundo JavaScript. No caso, é através da variável button, aquela que recebeu o retorno de document.querySelector que temos acesso à TAG <button>. Existem outros termos técnicos para tudo o que aconteceu aqui, mas eles não nos ajudam com lógica de programação.

# Muito bem, agora que temos o botão, se quisermos que ele chame a função tchau quando for clicado, precisamos associar a função ao botão atribuindo a função à button.onclick. Mas cuidado, você deve fazer:

    button.onclick = tchau;

E não

    button.onclick = tchau();
# Este último chama a função tchau e como ela não retorna nada, o valor de button.onclick será undefined. Além disso, como foram usados os () na chamada da função, ela será executada antes mesmo de clicarmos no botão. É por isso que fazemos:

    button.onclick = tchau;

#  ------------------------------------------------------------ #

# Ao longo do curso, aprendemos a lidar com tipos diferentes como, texto, número e booleano (ex.: 'true' ou 'false'). Exemplos desses tipos são:
var nome = "Regina"; // texto, ou tecnicamente falando, uma string
var idade = 22; // número
var temCarteira = true; // booleano