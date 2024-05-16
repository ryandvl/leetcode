# Problema

Escreva uma função para encontrar a cadeia de prefixo comum mais longa em uma array de strings.

Se não houver um prefixo comum, retorne uma string vazia `""`.

## Exemplos

> Entrada: `strs = ["flower","flow","flight"]`

> Saída: `"fl"`

** **

> Entrada: `strs = ["dog","racecar","car"]`

> Saída: `""`

> Explicação: Não há um prefixo comum entre os `input strings`.

## Sobre a minha Solução

A solução mais rápida que encontrei tem limitações mas funciona dependendo dos elementos, primeiro vamos usar o método `sort` na array para deixar todos elementos na ordem alfabética, com isso todos elementos que começarem com os mesmos prefixos ficarão seguidos, depois disso vamos percorrer cada caractere do primeiro elemento e comparar o primeiro caractere do primeiro elemento com o primeiro caractere do último elemento, caso eles sejam diferentes será retornado "" pois não foi encontrado nenhum, caso contrário o caractere será adicionado ao resultado. Após isso será retornado o resultado.

### Pontos-chave

- Nesta solução o tempo tem que ser O(n * m)

### Códigos

> Linguagens em que fiz essa Solução: `JavaScript`, `Python`, `Java` e `C++`.

Os códigos estão disponíveis em [codes.md](./codes.md).