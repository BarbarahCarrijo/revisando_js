# Revisando ou Iniciando com JS
Exercícios básicos de JS para aprendizado, fixação e revisão de conceitos da linguagem JavaScript

# Ementa

## Variáveis e tipos de dados

### Variáveis?

As variáveis, são espaços de memória no computador onde podemos armazenar distintos tipos de dados.

### Declaração de variáveis

Em programação uma variável é um espaço na memória do computador, que podemos usar para armazenar valores.
Se quisermos usar uma variável, a primeira coisa que devemos fazer é declará-la, isto é, criar essa "caixa" onde armazenaremos os valores.
Em JavaScript, as variáveis são declaradas usando a palavra var seguido do nome com o qual iremos identificá-lo.

Por exemplo:

~~~javascript
var preco
~~~

Temos algumas regras para criar nome de variaveis:

* Não pode começar com número
* Não pode ter caracteres especiais
* Não pode utilizar acentos
* Não pode utilizar espaços
* Deve começar com letra minuscula e seguir o padrão camelCase, onde cada palavra é iniciada com maiúsculas e unidas sem espaços.

### Armazenando dados

Nós já vimos como declarar uma variável. Agora precisamos atribuir um valor à ela.
Para salvar um valor em uma variável, usamos o sinal = e, em seguida, o valor que queremos armazenar.

Por exemplo:

~~~javascript
var meses = 12
var quantidadeDeAlunos = 30
~~~

Você pode ter visto em JavaScript alguns comandos, instruções que terminam em ";".
Em Javascript, o sinal ";" é opcional. Mas é importante que você utilize para o computador conseguir entender onde termina o comando.

Para começar, no exercício anterior vimos:

~~~javascript
var meses = 12
var quantidadeDeAlunos = 30
~~~

Também poderia ter sido escrito da seguinte forma, como abaixo:

~~~javascript
var meses = 12;
var quantidadeDeAlunos = 30;
~~~

### Variáveis e Operações

Vimos como declarar uma variável e atribuir um valor a ela e, provavelmente, agora você se pergunta, e qual é a utilidade de armazenar dados em variáveis?
As variáveis nos permitem reutilizar os dados atribuídos, simplesmente invocando seu nome.

~~~javascript
var numero  = 124;
console.log(numero); 
// Podemos usar console.log para imprimir o valor que tem atribuído à variável numero. E seu resultado será 124.
~~~

Algo muito importante também, é, assim como podemos fazer operações matemáticas como adicionar (+) ou subtrair (-) números, podemos fazer o mesmo com as variáveis que os referenciam.
Por exemplo:

~~~javascript
var numero = 124;
var numeroSeguinte = numero + 1;
console.log(numeroSeguinte); 
// O resultado que será impresso na tela será o valor atribuído a variável numero somado a 1, portanto, o valor atribuído a numeroSeguinte será 125.
~~~

Vamos ver se está entendido: Declare e atribua duas variáveis, `numeroA` e `numeroB`, e então nas variáveis `resultadoSoma`, `resultadoSubtracao`, `resultadoMultiplicacao` e `resultadoDivisao` armazene os cálculos feitos utilizando `numeroA` e `numeroB` nas variáveis de resultado, de modo que o cálculo matemático se altere de acordo com o título da variável, por exemplo. Exemplo `var resultadoSoma = (numeroA + numeroB)` Como nossa variável `resultadoSoma` indica nós devemos fazer uma soma utilizando as variáveis `numeroA` e `numeroB`. Para testar a sua resolução, você precisa apenas executar a sua resposta.

Exemplos:
soma: a + b
subtração: a - b
multiplicação: a * b
divisão: a / b

*Resposta*

~~~javascript
var numeroA = 20;
var numeroB = 5;
var resultadoSoma;
var resultadoSubtracao
var resultadoMultiplicacao
var resultadoDivisao

resultadoSoma = numeroA + numeroB;
resultadoSubtracao = numeroA - numeroB;
resultadoMultiplicacao = numeroA * numeroB;
resultadoDivisao = numeroA / numeroB;

console.log(resultadoSoma);
console.log(resultadoSubtracao);
console.log(resultadoMultiplicacao);
console.log(resultadoDivisao);
~~~

### Outro tipo de dado


Além dos números, há mais um tipo de dados em JavaScript.
Este tipo de dado é:

 `String`

Os dados do tipo String são conhecidos como cadeia de caracteres e nos permitem representar qualquer combinação de letras, números e/ou símbolos.
Para definir uma string, é necessário que o texto em questão esteja entre aspas:

~~~javascript
"João"
"Meu nome é João"
"125 + 125 = 250!"
~~~

Para gerar uma String, posso simplesmente atribuir o texto a uma variável; por exemplo:


~~~javascript
var meuPlaneta = "Terra";
console.log(meuPlaneta) //Isto irá imprimir na tela “Terra"
~~~

> Para passar para o próximo exercício, declare a variável `saudacao` e atribua o texto "Hello World".  E finalmente imprima o valor da variável na tela usando o `console.log`

*Resposta*

~~~javascript
var saudacao = "Hello World";
console.log(saudacao)
~~~


### Mais operações

### Outras operações

### Trocar valores

### Mais tipos de dados

### Mais sobre os booleanos
