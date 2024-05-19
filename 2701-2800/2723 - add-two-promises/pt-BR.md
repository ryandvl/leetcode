# Problema

Dadas duas promessas `promise1` e `promise2`, retorne uma nova promessa. `promise1` e `promise2` serão ambas resolvidas com um número. A promessa retornada deve ser resolvida com a soma dos dois números.

## Exemplos

> Entrada:
> ```
> promise1 = new Promise(resolve => setTimeout(() => resolve(2), 20)),
> promise2 = new Promise(resolve => setTimeout(() => resolve(5), 60))
> ```

> Saída: `7`

> Explicação: As duas promessas de entrada são resolvidas com os valores `2` e `5`, respectivamente. A promessa retornada deve ser resolvida com um valor de `2 + 5 = 7`. O tempo de resolução da promessa retornada não é avaliado para esse problema.

** **

> Entrada:
> ```
> promise1 = new Promise(resolve => setTimeout(() => resolve(10), 50)), 
> promise2 = new Promise(resolve => setTimeout(() => resolve(-12), 30))
> ```

> Saída: `-2`

> Explicação: As duas promessas de entrada são resolvidas com os valores `10` e `-12`, respectivamente. A promessa retornada deve ser resolvida com um valor de `10 + -12 = -2`.

## Sobre a minha Solução

Usar o método `Promise.all` nas duas arrays para ter os dois números de entrada, e depois fazer a soma dos dois.

### Pontos-chave

- Usar o método `Promise.all` para obter o resultado esperado.

### Códigos

> Linguagens em que fiz essa Solução: `JavaScript` e `TypeScript`.

Os códigos estão disponíveis em [codes.md](./codes.md).