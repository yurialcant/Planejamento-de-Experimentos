# Planejamento-de-Experimentos
Projeto criado durante a Aula de Planejamento de Experimentos.

# Projeto Pandas Alura
| 🪧 Vitrine.Dev |     |
| -------------  | --- |
| ✨ Nome        | Planejamento de Experimentos
| 🏷️ Tecnologias | Python, Pandas, matplotlib, Scipy, Seaborn
| 🚀 URL         | https://github.com/yurialcant/Planejamento-de-Experimentos
| 🤿 Desafio |https://cursos.alura.com.br/course/analise-de-experimentos

<h1 align ="center"> Análise de experimentos </h1>
<p align="center">
<img src="http://img.shields.io/static/v1?label=STATUS&message=%20COMPLETO&color=GREEN&style=for-the-badge"/>
</p>

![](https://user-images.githubusercontent.com/102321564/207418663-1c12134a-247f-4d7a-bae6-3b04142a8761.png#vitrinedev)

Este projeto foi criado durante o curso de Análises de Experimentos, nele utilizamos diversas bibliotecas como pandas, scipy, matplotlib e seaborn, utilizamos o jupyter notebook,
dentro do Visual Studio Code, o intuito desse experimento era ajudar a dona de uma loja de cupcakes a utilizar uma determinada quantia de farinha e de chocolate para uma quantia
desejada de cupcakes.

<h1 align ="center"> Resultados Obtidos </h1>

<h1>Importando Bibliotecas</h1>
<h2>Construindo o DataFrame</h2>

Iniciamos importando as bibliotecas que usuremos de imediato no projeto, sendo elas o pandas, numpy e pyDoe2, construimos um planejamento fatorial usando o método doe e inserimos em um Data Frame.


![Captura de Tela (278)](https://user-images.githubusercontent.com/102321564/207662712-f67103b1-0924-4ef0-bd1e-55fdda7fe96c.png)

Logo em seguida analisamos de maneira gráfica nosso Data Frame e para isso importamos o seaborn e construímos 2 gráficos, um dedicado para a farinha e outro para o chocolate.

![Captura de Tela (279)](https://user-images.githubusercontent.com/102321564/207663477-5900c35c-7fa0-421c-a9af-c952dc31fab3.png)

<h1>Modelo Estatístico</h1>
<h2>Análise de Significância Estatística</h2>

Então começamos a construir nosso modelo estatístico, para isso importamos a biblioteca statsmodel e usamos o método ols, para passarmos nossa fórmula que será utilizada, depois ajustamos o modelo com o método fit e por fim usamos o método summary para obtermos mais informações estatísticas sobre nosso modelo.

![Captura de Tela (280)](https://user-images.githubusercontent.com/102321564/207664392-21b2806c-cc8f-40da-98d7-72f6a17b14b4.png)

Optamos por aumentar nosso grau de liberdade e portanto criamos um novo Data Frame, desta vez com mais 4 itens e nos utilizamos do método append, para juntarmos este novo Data Frame ao anterior.

![Captura de Tela (281)](https://user-images.githubusercontent.com/102321564/207665055-4a852d02-4354-4ce2-9538-8d62b7711ce1.png)

Agora novamente iremos realizar a análise de significância estatística, com o método summary e notamos que os elementos que são significantes são o Intercept, a Farinha e o Chocolate, pois são menores que nosso alfa (Em nosso projeto o alfa considerado foi o de %).

![Captura de Tela (282)](https://user-images.githubusercontent.com/102321564/207666149-5bf4f425-c936-4841-8414-b3253e2e3ca7.png)

Para comprovar os valores de significância nos utilizamos da biblioteca do scipy, para construirmos nosso diagrama de pareto.

![Captura de Tela (283)](https://user-images.githubusercontent.com/102321564/207666707-681a3813-74ed-4194-b5c7-446f01618620.png)

Com isso construimos um novo modelo estatístico, utilizando somente as variaveis significantes, ajustamos o modelo e realizamos o método summary novamente.

![Captura de Tela (284)](https://user-images.githubusercontent.com/102321564/207667060-197cd9a7-6de3-4a5d-ae17-a86b0d9ff6e0.png)

Construímos novamente um novo gráfico de pareto, agora somente com as variaveis significantes.

![Captura de Tela (285)](https://user-images.githubusercontent.com/102321564/207667403-7d3ff326-774a-4802-ac38-74513d7e2007.png)

<h1>Definindo a Função</h1>

Neste momento, definimos uma função, para que nossa cliente possa inserir a quantidade de farinha e de chocolate que ela deseja usar e ter como resultado a quantidade de cupcakes que serão obtidos.

![Captura de Tela (286)](https://user-images.githubusercontent.com/102321564/207668178-25116830-52b6-4905-868f-2d0a240c74f3.png)

<h1>Criando Mapa de Cores</h1>
<h2>Utilizando Matplotlib</h2>

E por criamos um mapa de cores utilizando o matplotlib, onde primeiro definimos os pontos do nosso mapa, para podermos inseri-los em nosso mapa, nos utilizando dos métdoso imshow e contour.

![Captura de Tela (289)](https://user-images.githubusercontent.com/102321564/207669307-bd10fe16-130a-4c08-ace9-57b65bed73ea.png)

![Captura de Tela (288)](https://user-images.githubusercontent.com/102321564/207669051-e30a3363-70f2-47d7-8697-0e68a2b8e31b.png)










