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
* Deve começar com letra minúscula e seguir o padrão camelCase, onde cada palavra é iniciada com maiúsculas e unidas sem espaços.

### Armazenando dados

Nós já vimos como declarar uma variável. Agora precisamos atribuir um valor à ela.
Para salvar um valor em uma variável, usamos o sinal `=` e, em seguida, o valor que queremos armazenar.

Por exemplo:

~~~javascript
var meses = 12
var quantidadeDeAlunos = 30
~~~

Você pode ter visto em JavaScript alguns comandos, instruções que terminam em `;`.
Em Javascript, o sinal `;` é opcional. Mas é importante que você utilize para o computador conseguir entender onde termina o comando.

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

> Vamos ver se está entendido: Declare e atribua duas variáveis, `numeroA` e `numeroB`, e então nas variáveis `resultadoSoma`, `resultadoSubtracao`, `resultadoMultiplicacao` e `resultadoDivisao` armazene os cálculos feitos utilizando `numeroA` e `numeroB` nas variáveis de resultado, de modo que o cálculo matemático se altere de acordo com o título da variável, por exemplo. Exemplo `var resultadoSoma = (numeroA + numeroB)` Como nossa variável `resultadoSoma` indica nós devemos fazer uma soma utilizando as variáveis `numeroA` e `numeroB`. Para testar a sua resolução, você precisa apenas executar a sua resposta.

Exemplos:
soma: a + b;
subtração: a - b;
multiplicação: a * b;
divisão: a / b;

**Resposta**

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

**Resposta**

~~~javascript
var saudacao = "Hello World";
console.log(saudacao)
~~~


### Mais operações

E o que acontece se eu quiser unir textos?  Neste caso, o símbolo + nos ajudará a concatenar, isto é, juntar nossas strings.

FIQUE DE OLHO, NÃO ESQUEÇA OS ESPAÇOS!

Vamos tentar:

~~~javascript
var nome = "Ronaldo";
var nacionalidade = "Brasileiro";
console.log(nome + " é " + nacionalidade) 
// O resultado seria: "Ronaldo é Brasileiro"
~~~

E o que acontece se eu adicionar números com textos?

~~~javascript
var rua = "Av Paulista";
var numero = 1578;
console.log (rua + " " + numero)
// O resultado seria: "Av Paulista 1578"
~~~

Como você viu, se eu adicionar um número e um texto, ele se tornará parte da string.

> Declarar e atribuir três variáveis, uma com `nome`, outra com `sobrenome` e outra com `idade`. Então, declare uma variável com `nome` resultado e atribua uma string unindo suas variaveis da seguinte forma: " João Silva terá 30 anos" e utilize o `console.log` pra mostrar o que acontece. Respeite os espaços!

**Resposta**

~~~javascript
var nome = "Bárbara";
var sobrenome = "Carrijo";
var idade = 26;
var resultado = nome + " " + sobrenome + " terá " + idade + " anos" 

resultado = nome + " " + sobrenome + " terá " + idade + " anos" 

console.log (resultado);
~~~


### Trocar valores

As variáveis além de armazenar informações, e como seu nome diz, podem variar o valor que armazenam. Por exemplo:

~~~javascript
vencedor = "Pelé";
vencedor = "Marta";
console.log (vencedor);
//  resultado seria: "Marta"
~~~

Como você deve ter notado, chamando a variável e fazendo uma reatribuição a um valor eu posso mudar seu conteúdo.

> Vamos ver se entendeu: Defina a variável `numeroA` com um valor de 30 e defina a variável `numeroB` com um valor de 45. Em seguida, faça a variável `numeroA` armazenar o valor da variável `numeroB` e vice-versa. </br>
> *Dica: Neste procedimento, você precisa criar uma terceira variável chamada de `numeroC` para auxiliar.*

**Resposta**

~~~javascript
var numeroA = 30;
var numeroB = 45;
var numeroC;

numeroC = numeroA + numeroB;
numeroA = numeroC - numeroA;
numeroB = numeroC - numeroB;

console.log(numeroA);
console.log(numeroB);
console.log(numeroC);
~~~


### Mais tipos de dados

Já vimos os valores numéricos e as strings, mas em JavaScript há mais um tipo de dado:

`Booleano`

O Boolean é conhecido como booleano e permite representar dois valores lógicos, são eles:

* `true`: Representa o valor de algo ser verdadeiro
* `false`: Representa o valor de algo sendo falso

Para gerar um booleano, posso simplesmente atribuir o valor true ou false a uma variável.

Por exemplo:

~~~javascript
var valorVerdadeiro = true;
console.log (valorVerdadeiro) // Isso irá imprimir "true" na tela
~~~

> Para continuar, defina uma variável `gostoDeSorvete` e atribua a ela um valor booleano. Então, utilize `console.log(gostoDeSorvete)` para ver o que acontece!

~~~javascript
var gostoDeSorvete = true
console.log (gostoDeSorvete);
~~~


### Mais sobre os booleanos

O poder real dos booleanos é que eles podem surgir ao fazer comparações de valores diferentes com alguns operadores matemáticos.

Por exemplo, sabemos que se perguntarmos a alguém "2 é maior que 1?" a pessoa nos dirá "Sim é verdade, 2 é maior que 1", o mesmo acontece em JavaScript quando escrevemos o seguinte:

~~~javascript
console.log(2 > 1) // Isso imprimirá "true" na tela
~~~

Isso significa que "2 > 1" tem um valor de true. Nós também poderíamos ter escrito o mesmo código da seguinte forma

~~~javascript
var valorVerdade  = 2 > 1; 
// Como vimos 2> 1, ele retorna um valor de verdade e o atribuímos a uma variável
console.log (valorVerdade) // Isso imprimirá "true" na tela
~~~

E se perguntarmos a alguém "2 é menor que 1?" a pessoa dirá "Isso é falso, 2 não é menor que 1", o mesmo acontece em JavaScript quando escrevemos o seguinte:

~~~javascript
console.log(2 < 1) // Isso imprimirá "false" na tela
~~~

> Para continuar, defina duas variáveis: `umNumeroPequeno` e `umNumeroGrande`, e atribua a elas valores numéricos diferentes de acordo com seus nomes. Então defina a variável `eMenor` e atribua o resultado da comparação se `umNumeroPequeno` é menor do que `umNumeroGrande`; e defina a variável `eMaior`, com o resultado da comparação `umNumeroPequeno` é maior que `umNumeroGrande`.


**Resposta**


~~~javascript
var umNumeroPequeno = 10;
var umNumeroGrande = 100;
var eMenor;
var eMaior;

eMenor = umNumeroPequeno < umNumeroGrande;
eMaior = umNumeroPequeno > umNumeroGrande;

console.log(eMenor)
console.log(eMaior)
~~~

