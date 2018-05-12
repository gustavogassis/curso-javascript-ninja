# Desafio da semana #2

Nesse exercício, você está livre para escolher os nomes para suas variáveis e funções! :smile:

```js
// Crie uma função que receba dois argumentos e retorne a soma dos mesmos.
function soma(a, b) {
  return a + b;
 }

// Declare uma variável que receba a invocação da função criada acima, passando dois números quaisquer por argumento, e somando `5` ao resultado retornado da função.
var x = soma(3, 7) + 5;

// Qual o valor atualizado dessa variável?
 15

// Declare uma nova variável, sem valor.
var y;

/*
Crie uma função que adicione um valor à variável criada acima, e retorne a string:
    O valor da variável agora é VALOR.
Onde VALOR é o novo valor da variável.
*/
function mudar(v) {
  y += v;
  return "O valor de y agora é " + v;

// Invoque a função criada acima.
mudar(70);

// Qual o retorno da função? (Use comentários de bloco).
/* "O valor de y agora é 70" */

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos;
2. Se qualquer um dos três argumentos não estiverem preenchidos, a função deve retornar a string:
    Preencha todos os valores corretamente!
3. O retorno da função deve ser a multiplicação dos 3 argumentos, somando `2` ao resultado da multiplicação.
*/
function multi(a, b, c) {
  if (a === undefined || b === undefined || c === undefined) {
    return 'Preencha todos os valores corretamente!';
  }
  return ( a * b * c) + 2;
}

// Invoque a função criada acima, passando só dois números como argumento.
multi(3,5);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
// "Preencha todos os valores corretamente!"

// Agora invoque novamente a função criada acima, mas passando todos os três argumentos necessários.
multi (4, 5, 0);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
// O valor retornado será 5

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos.
2. Se somente um argumento for passado, retorne o valor do argumento.
3. Se dois argumentos forem passados, retorne a soma dos dois argumentos.
4. Se todos os argumentos forem passados, retorne a soma do primeiro com o segundo, e o resultado, dividido pelo terceiro.
5. Se nenhum argumento for passado, retorne o valor booleano `false`.
6. E ainda, se nenhuma das condições acima forem atendidas, retorne `null`.
*/ ab ac bc
function ninja(a, b, c) {
  if (a !== undefined && b === undefined && c === undefined) {
    return a;
  }
  
  if (b !== undefined && a === undefined && c === undefined) {
    return c;
  }
  
  if (c !== undefined && a === undefined && b === undefined) {
    return c;
  }
  
  if (a !== undefined && b !== undefined && c === undefined) {
    return a + b;
  }
  
  if (a !== undefined && c !== undefined && b === undefined) {
    return a + c;
  }
  
  if (b !== undefined && c !== undefined && a === undefined) {
    return b + c;
  }
  
  if (a !== undefined && b !== undefined && c !== undefined) {
    return (a + b) / c;
  }
  
  if (a === undefined && b !== undefined && c !== undefined) {
    return false;
  }
  
  return "null";
}

// Invoque a função acima utilizando todas as possibilidades (com nenhum argumento, com um, com dois e com três.) Coloque um comentário de linha ao lado da função com o resultado de cada invocação.
ninja(); // false
ninja(4); // 4
ninja(5,7); // 12
ninja(4,6,2); // 5
```
