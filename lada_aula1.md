### introdução a programação, em python `:)`
Python é uma linguagem de programação de proposito geral e facil de aprender,
e pra ficar mais facil ainda as ferramentas necessarias serão somente ter internet
e um navegador, vamos usar [https://www.online-python.com/](https://www.online-python.com/)

##### sobre o [online-python](https://www.online-python.com/):
possui duas areas pra inserir texto, o primeiro é onde será colocado o codigo e o segundo
é usado para mostrar a saida gerada pelo codigo, em um ambiente de programação mais tradicional
a primeira tela seria um editor de texto qualquer e a segunda tela seria o console onde o codigo
é executado e mostrado o resultado dele
> apos inserir o codigo no site, pra executar aperte o botão __"Run"__


acho que ja ta bom, bora pro codigo!
#### python
```python
print('olá mundo')
```
> esse é um classico de todo iniciante em programação, praticamente um rito de passagem,
> essa linha tem um comando chamado `print`, o que esse comando faz é pegar o dado que está
> entre parentesis e imprimir na tela, essa tela no caso é o console ou o segundo painel
> lá do site

mas esse codigo é simples demais, bora pra algo um pouco mais elaborado
```python
ano_atual = int(input('qual o ano atual?: '))
ano_nascimento = int(input('qual o ano que voce nasceu?: '))

idade = ano_atual - ano_nascimento

print(f'sua idade é: {idade} anos')
```
> faça um teste, copie esse codigo e cole la no site

programação é escrever um roteiro para o computador seguir, uma receita de bolo, programação
nada mais é do que uma serie de comandos em que o computador vai ler cada linha e seguir o que
o comando diz

no codigo de exemplo acima, a primeira linha eu perguto ao usuario o ano atual, armazeno isso
em uma variavel, na segunda linha eu faço a mesma coisa so que perguntando o nascimento, no
proximo comando eu faço uma mera subtração e o resultado disso eu coloco em outra variavel

e pra finalizar, eu imprimo uma mensagem na tela contendo o valor guardado na variavel
> "ceerto, to acompanhando, mas que diabo é uma variavel?", essa seria uma excelente pergunta

#### Variaveis
podemos dizer que variaveis são objetos que guardam uma informação, e existe varios tipos
de variaveis, a gente classifica elas de acordo com o tipo de dado que ela guarda,

###### em python os principais tipos são:
* `int`: guarda numeros, 0, -1, 2, 6 etc
* `float`: guarda numeros com cada decimal, 1.6, 1.7 etc. Note que é usado ponto e não a virgula pra definir a casa decimal
* `str`: strings, que são textos delimitados por aspas, que pode ser tanto `"aspas duplas"` quanto `'aspas simples'`
* `bool`: o famigerado booleano, esse tipo guarda dois valores que seriam "verdadeiro" ou "falso" mas não os dois ao mesmo tempo (até porque não é o gato de schrödinger kk)
> eu especifiquei que isso é de python porque em outras linguagens de programação pode haver mais tipos de variaveis, com regras e limites sobre o uso de cada, mas a grosso modo se resume a isso

a sintaxe (regra, estilo etc) basica de declarar uma variavel é `nome_da variavel = um_dado_qualquer`
```python
um_numero = 42
um_float = 3.14
uma_string = 'humberto, doisberto'
um_booleano = True
```

nas proximas aulas será ensinado blocos de codigo, que seriam condicionais e blocos de repetição,
isso serve pra agrupar trechos de codigos e mudar o comportamento do programa baseado em alguma
regra o circustancia

#### exemplo de um uso pratico usando programação
o Youtube tem um player de video chamado shorts usado pra videos curtos, eu acho esse player muito
limitado em comparação ao tradicional, pra substituir o player basta pegar a url do video e
substituir a palavra `shorts` por `watch?v=` assim:
* [https://youtube.com/shorts/gv26oVXX7Hk?si=5rbC6NG7ec261it0](https://youtube.com/shorts/gv26oVXX7Hk?si=5rbC6NG7ec261it0)
* [https://youtube.com/watch?v=gv26oVXX7Hk?si=5rbC6NG7ec261it0](https://youtube.com/watch?v=gv26oVXX7Hk?si=5rbC6NG7ec261it0)

mas fazer isso toda vez manualmente é chato e propenso a erros, bora fazer o computador trabalhar pra gente
```python
url = input('qual a url?: ')
nova_url = url.replace('shorts', 'watch?v=')
print(f'nova url: {nova_url}')
```
> pegue um video shorts do yt e teste esse codigo naquele site mencionado no começo
