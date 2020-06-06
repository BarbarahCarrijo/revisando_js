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

Já vimos que podemos fazer cálculos matemáticos simples e de maior complexidade.

Agora vamos para algo mais interessante.

Queremos criar funções que nos permitam calcular a área e o perímetro de um círculo.

Vamos criar uma função perimetro que nos diga o perímetro de um círculo quando damos a ele o raio como parâmetro.

Também a função area que nos dá a área de um círculo quando recebe o raio como parâmetro. 

Lembre-se de usar o valor de 3.14 no lugar do π .

### Operando strings

### Criando cartões

### Conhecendo funções Math

### Mais uma função