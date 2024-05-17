# Problema

Dada uma string `s` contendo apenas os caracteres `'('`, `')'`, `'{'`, `'}'`, `'['` e `']'`, determine se a string de entrada é válida.

Uma string de entrada é válida se:

1. Parênteses abertos devem ser fechados pelo mesmo tipo de parênteses.
2. Parênteses abertos devem ser fechados na ordem correta.
3. Cada parêntese de fechamento tem um parêntese de abertura correspondente do mesmo tipo.

## Exemplos

> Input: `s = "()"`

> Output: `true`

** **

> Input: `s = "()[]{}"`

> Output: `true`

** **

> Input: `s = "(]"`

> Output: `false`

## Sobre a minha Solução

Percorrer a string e utilizar stack para guardar todos caracteres que são algum desses caracteres `([{` se o caractere não for um desses entraremos em uma outra verificação onde se o último elemento da stack não for a chave de abrimento e o caractere for a chave de fechamento retorna false, se não apenas removendo o último elemento da array pois foi fechado com sucesso. Com isso, no final basta verificar o tamanho de itens na stack, se estiver vazia teve sucesso.

### Pontos-chave

- Reduzir o tempo para O(1) em vez de O(N).

### Códigos

> Linguagens em que fiz essa Solução: `JavaScript`, `Python`, `Java` e `C++`.

Os códigos estão disponíveis em [codes.md](./codes.md).