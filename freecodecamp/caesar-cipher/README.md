# Caesar Cipher

Exercício da certificação Scientific Computing with Python (freeCodeCamp).

## Como funciona

A função `caesar()` desloca cada letra do texto um número fixo de posições
no alfabeto (o `shift`), usando `str.maketrans` + `str.translate` para
trocar todos os caracteres de uma vez, sem precisar de loop manual.

Pra descriptografar, uso o mesmo shift só que negativo — assim não preciso
duplicar a lógica de rotação em duas funções diferentes.

## Validações

- Só aceita `shift` inteiro entre 1 e 25 (fora disso, uma letra criptografada
  vira ela mesma ou "roda demais" e some o sentido da cifra).

## Exemplo

    encrypt("Hello, World!", 5)  -> "Mjqqt, Btwqi!"
    decrypt("Mjqqt, Btwqi!", 5)  -> "Hello, World!"
