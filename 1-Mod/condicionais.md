## Condicionais

### Operadores lógicos

Vamos lembrar a definição de operadores:
“Os operadores nos permitem manipular o valor das variáveis, realizar operações e comparar seus valores”

OPERADORES LÓGICOS
Permitem combinar valores booleanos, o resultado também devolve um booleano.
Existem três operadores e (and), ou (or), negação (not).

AND (&&) todos los valores devem retornar como true
OR ( || ) ao menos um valor deve evaluar como true.
NOT ( ! ) nega a condição, se era true, será false e vice-versa

As operações com operadores lógicos sempre devolverá um booleano, ou seja, retorna true ou false, como resultado.

### Condicionais

Tomamos decisões o tempo todo em nossa vida, dependendo de diferentes condições.
Na programação, podemos fazer o mesmo. Convidamos você a aprender como  fazemos assistindo a este vídeo que fala sobre **condicionais**.

Nos permitem avaliar as condições e realizar diferentes ações de acordo com o resultado dessas avaliações.

CONDICIONAL SIMPLES

~~~javascript
if (condicao) {
 // código a executar se a condição for verdadeira
}
~~~

CONDICIONAL COM ELSE

~~~javascript
if (condicao) {
 // código a executar se a condição for verdadeira
} else {
 // código a executar se a condição for falsa
}
~~~

CONDICIONAL COM ELSE IF

~~~javascript
if (condicao) {
 // código a executar se a condição for verdadeira
} else if (outra condição) {
 // código a executar se a condição for verdadeira
} else {
 // código a executar se a condição for falsa
}
~~~

**Código de Exemplo:**

~~~javascript
let idade = 19;
let acesso = '';

if (idade < 16) {
  acesso = 'proibido';
} else if (idade >= 16 && idade <= 18) {
  acesso = 'permitido somente quando
acompanhado por um maior de idade';
} else {
  acesso = 'permitido';
}
~~~

*Explicação para o código apresentado:*

> Declaramos a variável idade e lhe atribuímos o número 19;
> Declaramos a variável de acesso e lhe atribuímos uma string vazia, com a intenção de atribuir-lhe um novo valor de acordo com o resultado dos condicionantes declarados abaixo.
> Iniciamos a condicional. Nossa primeira condição avalia se a idade é menor de 16 anos. Se for verdade, atribuímos a string 'proibido' à variável de acesso.
Neste caso, a condição é falsa, portanto o Javascript procede a avaliar a seguinte condição.
> Nós declaramos um else if para contemplar uma segunda condição:
Esta condição será composta e exigirá:
- que a idade seja maior ou igual a 16
- que a idade seja menor ou igual a 18
A condição é novamente falsa, então o Javascript continua a leitura da condicional.
Como nenhuma das condições acima era verdadeira, o código é executado dentro do else.
Portanto, a variável de acesso agora é igual à string 'permitido'.

*Dica:* É uma boa prática inicializar as variáveis com o tipo de dados que elas vão armazenar.

### Que tal se?

Nenhuma introdução a Javascript estaria completa sem mostrar a estrutura de controle condicional, conhecida como if.

O `if` nos permite executar um código de acordo com uma condição.

Um exemplo da vida real poderia ser: **Se o dia está ensolarado, vamos para a praia!** Como pode ver, no exemplo anterior estamos dando uma condição, a ida para a praia só acontecerá se o dia estiver ensolarado.

Muito bem, como podemos transcrever o que vimos para código? Primeiro devemos entender que o if se divide em 3 partes :

  1 - A palavra reservada `if`.
  2 - A condição que queremos validar, ela deve ficar entre parênteses **()**.
  3 - O bloco de código que é executado quando a condição se cumpre (ou seja quando ela é `true` -verdadeira-), e deve ficar entre chaves **{}**.

Vejamos um exemplo:

~~~javascript
let numero = 43;

if (numero > 0) {
    console.log('O número é positivo');
}
~~~

Agora como poderíamos resolver a condição da praia através do código?

Vamos ver:

~~~javascript
if (eDiaEnsolarado == true) {
    console.log('Vamos para praia!');
}
~~~

No exemplo anterior, `eDiaEnsolarado` seria uma variável que armazena um valor booleano, e sempre que esse valor for exatamente igual a `true`, vamos executar bloco de código que se encontra dentro das chaves `{}`, nesse caso, o `console.log`.

Vamos fazer uma pequena prática para ir entendendo o conceito.

> Declara a variável `diaDeSemana` que receba uma string `"domingo"`. Depois implemente uma condicional usando o `if` que compare se `diaDeSemana` é igual a `"domingo"`, se for verdadeiro imprima uma string `"Hoje é dia de futebol!!!"`.
Lembre-se que as variáveis e as strings devem ser escritas igual ao enunciado, respeitando os espaços e as exclamações.


*Dica:* Quando comparamos valores utilizamos o sinal de igual duas vezes ==.

**Resposta**

~~~javascript
var diaDeSemana = "domingo"

if (diaDeSemana === "domingo") {
    console.log("Hoje é dia de futebol! ! !");
}
~~~

### E que tal se não?


### Qual é maior?

### Qual é o seu sinal?

### O número da sorte

### Posso ir ao banco?

### O filósofo hipster

### As tabelas verdade

### Voltando à escola

### Um exercício sem precedentes

### Nós vamos ao parque de diversões

### Agora vamos ter dar um prêmio
