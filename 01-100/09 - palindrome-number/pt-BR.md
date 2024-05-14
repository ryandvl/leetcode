# Problema

Dado um número inteiro `x`, retorne `true` se `x` for um **palíndromo** e `false` caso contrário.

Um número inteiro é um palíndromo quando tem a mesma leitura para frente e para trás.

Por exemplo, `121` é um palíndromo, enquanto `123` não é.

## Exemplos

> Entrada: `x = 121`

> Saída: `true`

> Explicação: `121` é lido como `121` da `esquerda para a direita` e da `direita para a esquerda`.

** **

> Entrada: `x = -121`

> Saída: `false`

> Explicação: Da `esquerda para a direita`, lê-se `-121`. Da `direita para a esquerda`, ele se torna `121-`. Portanto, não é um **palíndromo**.

** **

> Entrada: `x = 10`

> Saída: `false`

> Explicação: Lê-se `01` da `direita para a esquerda`. Portanto, não é um **palíndromo**.

## Sobre a minha Solução

Percorrer por cada digito do número todo, a cada índice verificamos se o índice da ordem contrária é o mesmo do atual, com isso podemos retornar `false` diretamente caso não sejam os mesmos, e números menores que `0` sempre serão `false`.

### Pontos-chave

- Podemos verificar se o digito `tamanho de x` menos a `índice atual` são os mesmos digitos.
- Reduzir o tempo para O(1) em vez de O(N).

### Códigos

> Linguagens em que fiz essa Solução: `JavaScript`, `Python`, `Java` e `C++`.

Os códigos estão disponíveis em [codes.md](./codes.md).