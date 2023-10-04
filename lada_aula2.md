
### introdução a programação, em python `:)` - DLC da aula passada
continuando a partir de onde parou da aula passada, nessa vamos aprender alguns fundamentos mais elaborados da programação que são blocos de codigos, `IFs`, `IF-ELSE` e `WHILE`

##### nesse vamos usar duas ferramentas pra testar as coisas:
* [https://www.online-python.com/](https://www.online-python.com/) - usado na aula passada
* [https://www.pythonsandbox.com/turtle](https://www.pythonsandbox.com/turtle)

já temos o necessario então vamos pro codigo!

#### blocos condicionais - `IFs` e `IF-ELSE`:
esse tipo de bloco verifica uma condição, e depedendo do resultado dessa verificação, ele pode ou não executar o comando que está dentro do bloco, ou ate mesmo não executar o comando pre definido e sim outro

```python
if condição:
    comando1
    comando2
```
```python
if condição:
    comando
else:
    outro_comando
```
```python
idade = 16

if idade > 18:
    print('não pode dirigir')
else:
    print('ja pode dirigir')
```

#### blocos de repetição - WHILE`:
> tambem conhecidos como laços de repetição ou loop

assim como os blocos anteriores, esses tambem verificam uma condição, a diferença desses é que se a condição verificada for valida, for considerada verdadeira, os comandos dentro do bloco serão executados mais de uma vez, e so vai parar de repetir quando a condição deixar de ser verdadeira

```python
while condição:
    comando
```
```python
numero = 247
divisor = 2

while divisor < numero:
    if numero % divisor == 0:
        print(f'o numero {numero} nao é primo')
        print(f'é divisivel por {divisor}')
        break

    divisor = divisor + 1
```

#### colinha de operadores de comparação
| operador | sintaxe | significado            |
|----------|---------|------------------------|
| ==       | x == y  | x é igual a y          |
| !=       | x != y  | x é diferente de y     |
| <        | x <  y  | x é menor que y        |
| >        | x >  y  | x é maior que y        |
| <=       | x <= y  | x é menor ou igual a y |
| >=       | x >= y  | x é maior ou igual a y |

#### colinha de operadores logicos
| operador | sintaxe | significado |
|----------|---------|-------------|
| and      | x and y | x e y       |
| or       | x or y  | x ou y      |

#### tabela verdade
##### operador `and`
|   |   |   |   |   |
|---|---|---|---|---|
| V | e | V | = | V |
| V | e | F | = | F |
| F | e | V | = | F |
| F | e | F | = | F |
##### operador `or`
|   |   |   |   |   |
|---|---|---|---|---|
| V | ou | V | = | V |
| V | ou | F | = | V |
| F | ou | V | = | V |
| F | ou | F | = | F |

#### desenhando com python turtle
turtle é uma biblioteca da linguagem python que permite criar desenhos simplesmente dando comandos que um "pincel" vai seguir, por exemplo, "ande tantos casas, vire tantos angulos e continue andando", o caminho que p pincel seguir ele vai marcando a tela

##### estrutura basica:
```pyhton
import turtle
t = turtle.Turtle()
```
##### principais comandos:
```python
t.right(90)     # vire a direita 90 graus
t.forward(100)  # ande 100 casas
t.left(90)      # vire a esquerda 90 graus
t.backward(100) # retroceda 100 casas
t.circle(60)    # desenhar um circulo com raio 60
```
