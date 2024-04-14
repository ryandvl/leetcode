# Problema

Dado um array de números inteiros `nums` e um número inteiro `target`, retorne os índices dos dois números de modo que eles somem para formar o `target`.

Você pode assumir que cada entrada terá exatamente uma solução e você não pode usar o mesmo elemento duas vezes.

Você pode retornar a resposta em qualquer ordem.

## Exemplos

> Entrada: nums = [2,7,11,15], target = 9

> Saída: [0,1]

> Explicação: Pois nums[0] + nums[1] == 9, retornamos [0, 1].

** **

> Entrada: nums = [3,2,4], target = 6

> Saída: [1,2]

** **

> Entrada: nums = [3,3], target = 6

> Saída: [0,1]

## Sobre a minha Solução

A solução mais fácil é percorrer pela array toda uma única vez, e durante o processo ir salvando os números em algo que vamos de Hashmap, se a diferença do número junto com o alvo é encontrado no Hashmap, e no passo final se for encontrado retorna `índice do número encontrado, índice atual`, o resultado foi encontrado.

### Pontos-chave

- Ao percorrer `nums` podemos utilizar `target - num` para detectar se existe um número que a diferença com o atual será o `target`.
- Usar Hashmap para salvar os indíces dos números que já foram percorridos.
- Reduzir o tempo para O(1) em vez de O(N).

### Códigos

> Linguagens em que fiz essa Solução: `JavaScript`, `Python`, `Java` e `C++`.

Os códigos estão disponíveis em [codes.md](./codes.md).