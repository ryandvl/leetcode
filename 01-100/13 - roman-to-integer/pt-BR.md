# Problema

Os números romanos são representados por sete símbolos diferentes: `I`, `V`, `X`, `L`, `C`, `D` e `M`.

> Símbolo | Valor
> -- | --
> I | 1
> V | 5
> X | 10
> L | 50
> C | 100
> D | 500
> M | 1000

Por exemplo, `2` é escrito como `II` em numeral romano, apenas dois uns somados juntos. `12` é escrito como `XII`, que é simplesmente `X + II`. O número `27` é escrito como `XXVII`, que é `XX + V + II`.

Os números romanos são geralmente escritos do maior para o menor da esquerda para a direita. No entanto, o numeral para quatro não é `IIII`. Em vez disso, o número quatro é escrito como `IV`. Porque o um está antes do cinco nós subtraímos ele fazendo quatro. O mesmo princípio se aplica ao número nove, que é escrito como `IX`. Existem seis instâncias onde a subtração é usada:

- `I` pode ser colocado antes de `V` (5) e `X` (10) para fazer 4 e 9.
- `X` pode ser colocado antes de `L` (50) e `C` (100) para fazer 40 e 90.
- `C` pode ser colocado antes de `D` (500) e `M` (1000) para fazer 400 e 900.

Dado um numeral romano, converta-o para um número inteiro.


## Exemplos

> Entrada: `s = "III"`

> Saída: `3`

> Explicação: `III = 3`.

** **

> Entrada: `s = "LVIII"`

> Saída: `58`

> Explicação: `L = 50, V= 5, III = 3`.

** **

> Entrada: `s = "MCMXCIV"`

> Saída: `1994`

> Explicação: `M = 1000, CM = 900, XC = 90 e IV = 4`.


## Sobre a minha Solução

Ao percorrer a string podemos verificar se o número romano atual é menor do que o próximo número romano, se for menor o resultado será diminuido na quantidade do romano atual, caso contrário será adicionado o número atual no resultado, e assim teremos o resultado.

### Pontos-chave

- Usar apenas os números romanos: I, V, X, L, C, D, M.
- Reduzir o tempo para O(1) em vez de O(N).

### Códigos

> Linguagens em que fiz essa Solução: `JavaScript`, `Python`, `Java` e `C++`.

Os códigos estão disponíveis em [codes.md](./codes.md).