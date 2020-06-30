## Funções

### O que são funções?

Uma função é um bloco de código que podemos invocar quantas vezes forem necessárias.
Pode realizar uma tarefa específica e retornar um valor.
Nos permite agrupar o código que vamos utilizar muitas vezes.

*Recomendação*
> Existem dois tipos de funções, as declaradas  e as expressadas, mas você está aprendendo e não queremos que se preocupe agora, e por isso recomendamos que use as funções declaradas.</br>
> Por exemplo:

~~~javascript
function dobro(numero) {
   return numero * 2;
}
~~~

### Declaração

Vamos começar com o básico:

As funções consistem em 4 partes. A palavra reservada `function`, o nome com o qual vamos chamar a função, os parênteses onde irá os parâmetros (Caso a função não precise de parâmetros, ainda sim, devemos colocar os parenteses), as `{}` chaves que dentro teremos o código que queremos que a função execute .

Se quisermos que uma função retorne um valor, precisaremos da palavra-chave `return`. Depois disso, tudo o que queremos irá retornar.

Com as funções, podemos fazer muitas coisas, mas vamos começar com algo fácil. Veja esse exemplo onde a função a seguir dobra o valor do número que passamos para ela:

~~~javascript
function dobro(numero) {
   return numero*2;
}
~~~

Como podemos ver, acima nós declaramos uma função com a palavra reservada `function` e o nome `dobro`. Entre os parênteses, colocamos o parâmetro `numero` que será substituído pelo número que damos ao fazer a chamada da função. Para terminar, com a palavra return dizemos que queremos que a função retorne 2 vezes o numero que lhe demos.

Para executar a função e fazer o que queremos, nós precisamos chamá-la pelo nome e digitar o número que desejamos usar entre os parênteses.

~~~javascript
dobro(5);   //Isto irá devolver 10
dobro(1.5); //E isto irá devolver 3
~~~

> Neste exercício, crie a função `dobro` tendo como base o exemplo acima. O objetivo é fixar o seu entendimento sobre a estrutura de declaração de uma função.

**Resposta**

~~~javascript
function dobro(numero) {
   return numero*2;
}
~~~


### Mais funções

Então, para montar uma função, há coisas que não podemos deixar de fora. A palavra `function`, o nome da função, os parâmetros dentro dos parenteses (se necessário), o codigo dentro das `{}` e um `return` dentro do código, se quisermos que ele retorne algo para nós.

> Vamos praticar juntos: escreva agora uma função `metade`, que pega um número como parâmetro e retorna sua metade.

**Resposta**

~~~javascript
function metade(numero) {
   return numero/2;
}
~~~

#### Fazendo contas

Nós já vimos os operadores matemáticos básicos `+`, `-`, `/` e `*`.

Agora podemos utilizar funções para fazer estas contas de uma forma mais fácil.

~~~javascript
function somar(numero1,numero2){
  return numero1 + numero2 ;
}
~~~

> Escreva a função `multiplicar` que receba dois parâmetros, multiplique-os e retorne o resultado da multiplicação.

**Resposta**

~~~javascript
function multiplicar(numero1,numero2){
  return numero1 * numero2 ;
}
~~~

### Usando funções

Tendo essas pequenas funções, podemos combiná-las para fazer coisas mais complexas.

Por exemplo, se quisermos somar dois números e depois multiplicá-los por 3, poderíamos fazê-lo da seguinte maneira:

~~~javascript
function somar (num1, num2) {
   return num1 + num2;
}

function triploDaSoma(num3, num4) {
   var resultadoDaSoma = somar(num3, num4);
   return resultadoDaSoma * 3;
}
~~~

Aqui vemos que tendo a função `somar()` definida, podemos chamá-la dentro de outra função (neste caso dentro da função `triploDaSoma()`), guardar o seu resultado da execução em uma nova variável e tornar o trabalho mais fácil.

> Agora pedimos que você declare uma função chamada `triploDaSoma()` que recebe dois parâmetros. Então você tem que adicionar ambos e retornar três vezes o valor do resultado da soma dos dois parâmetros. Para fazer isso, você já conta (mesmo que não veja declarado) com a função `triplo`, que recebe um parâmetro e retorna o valor dele multiplicado por três.

**Resposta**

~~~javascript
function triplo (num1, num2) {
   return num1 + num2;
}

function triploDaSoma(num3, num4) {
   var resultadoDaSoma = triplo(num3, num4);
   return resultadoDaSoma * 3;
}
~~~

### Fórmulas e funções

Já vimos que podemos fazer cálculos matemáticos simples e de maior complexidade. Agora vamos para algo mais interessante
Queremos criar funções que nos permitam calcular a área e o perímetro de um círculo.

> Vamos criar uma função `perimetro` que nos diga o perímetro de um círculo quando damos a ele o raio como parâmetro. Também a função `area` que nos dá a área de um círculo quando recebe o `raio` como parâmetro. Lembre-se de usar o valor de 3.14 no lugar do π.
> Aqui estão as fórmulas necessárias para as funções, além disso, para este exercício iremos considerar que o valor de π é 3.14. perimetro = π * raio * 2; area = π * raio * raio;

**Resposta**

~~~javascript
var raio = 5;

function perimetro (raio) {
    return 3.14 * raio * 2
}

 function area (raio) {
    return 3.14 * raio * raio
}
~~~

### Operando strings

E o que podemos fazer que não seja matemática? Podemos trabalhar com **strings**! E se você se recorda, as **strings** são um tipo de dados. Representamos as cadeias de texto escrevendo dentro de aspas (“ “) literalmente.

E o que podemos fazer então com as strings? Por exemplo, podemos calcular quantos caracteres existem no total, e para isso iremos utilizar um recurso chamado length, onde colocamos a **string** seguida de `.length`. Veja alguns exemplos:

~~~javascript
"biblioteca".length // devolve 10
"babel".length     // devolve 5
~~~

E lembre-se que também podemos somar **strings**! Embora que, o termo correto seja **concatenar**, ou seja, obter uma nova string juntando duas ou mais **strings**.

~~~javascript
"aa" + "bb"    // devolve "aabb"
"aa" + " " + "bb" // devolve "aa bb"
~~~

> Vamos testar: Iremos criar uma função chamada `tamanhoNomeCompleto`, que recebe um `nome` e um `sobrenome` como parâmetros, e que irá devolver o tamanho total, contando um espaço extra para separar ambos:

~~~javascript
tamanhoNomeCompleto("Enzo", "Silva")
//  devolve 10
~~~

> Não utilize nomes literais nos parâmetros da função, tente ser sempre o mais genérico possível. O método length fornece o comprimento de qualquer palavra em números, isto significa que você será capaz de fazer as contas com isso.

**Resposta**

~~~javascript
var nome = "Barbara";
var sobrenome = "Carrijo";

function tamanhoNomeCompleto ( nome, sobrenome) {
    nomeCompleto = nome + " " + sobrenome
    return nomeCompleto.length
}
~~~

> Para uma conferência importante, os organizadores nos pediram para escrever os cartões de identificação que cada participante terá. Para isso, temos que colocar seu nome, seu sobrenome e seu título (dr., dra., lic., etc) e montar uma única string.
> Escreva a função `escreverCartao`, que recebe como parâmetros um `titulo`, um `nome` e um `sobrenome` e retorna uma única string como resultado. Por exemplo:

~~~javascript
escreverCartao("Dra.", "Ana", "Pérez")
//"Dra. Ana Pérez"
~~~

> Lembre-se de não usar valores específicos ou literais nos parâmetros da função. Você também pode tentar concatenar espaços entre cada palavra.

**Resposta**

~~~javascript
var titulo = "Dra.";
var nome = "Ana";
var sobrenome = "Pérez";

function escreverCartao ( titulo,nome, sobrenome) {
    cartao = titulo + " " + nome + " " + sobrenome
    return cartao
}
~~~

### Conhecendo funções Math

Graças aos programadores de JavaScript, temos algumas funções que você pode usar sem declarar (porque eles fizeram isso por nós). Estas são algumas das funções matemáticas que podemos usar:

> `Math.abs ()` retorna o valor absoluto do número que passamos para ele como *parâmetro*.

~~~javascript
Math.abs (4) //retorna 4
Math.abs (0) //retorna 0
Math.abs (-123) //retorna 123
~~~

>  `Math.round ()` arredonda um número para cima até o número inteiro mais próximo e `Math.floor ()` arredonda um número para baixo até o número inteiro mais próximo.

~~~javascript
Math.round (4.6) //retorna 5
Math.round (4.3) //retorna 4
Math.floor (4.6) //retorna 4
Math.floor (4.3) //retorna 4
~~~

> `Math.max ()` pega dois parâmetros e retorna o maior número, enquanto `Math.min ()` pega dois parâmetros e retorna o menor.

~~~javascript
Math.max (4, 7) //retorna 7
Math.min (4, 7) //retorna 4
~~~

Além das funções vistas no exercício anterior, existe uma função já definida em JavaScript que é muito importante: `Math.random ()`. Essa função gera um número **aleatório** decimal entre 0 e 1, e é a base para muitos cálculos usados na programação.

~~~javascript
Math.random()
// exemplo de retorno 0.056

Math.random()
// exemplo de retorno 0.178
~~~

> Escreva uma função `gerarProbabilidade()`, que não recebe parâmetros e retorna a porcentagem de probabilidade de chuva, calculada aleatoriamente usando `Math.random ()`.

**Resposta**

~~~javascript
function gerarProbabilidade () {
    return Math.random ()
}
~~~
