# Calculadora de integrais com soma de Riemann

## Introdução da ideia do código:
O código mostrado aqui tem como objetivo calcular o valor aproximado de algumas integrais definidas dados como input pelo usuário, bem como o intervalo de integração. O código também define uma margem de erro aceitável para a aproximação. Para essa aplicação, a margem de erro utilizada foi de 10^-6.

## A ideia geral da integral:
Podemos, de forma mais resumida, definir a ideia geral da integral pelo objetivo de calcular a área abaixo da curva de uma função f(x).  
Dado esse objetivo, surgem algumas maneiras de se calcular essas áreas abaixo dessas funções, de tal maneira que é possível computar um valor aproximado para as integrais dessas funções. Por meio dessa série, abordando o conceito da aproximação desses valores por meio da soma de Riemann, destaco dessa aplicação em código python.

## Conceito de integral pela soma de Riemann:
Temos a ideia geral da integral definida, com base no livro de James Stewart, como sendo a seguinte:  

Dada uma função f contínua definida em a ≤ x ≤ b de intervalo, dividimos o intervalo [a, b] em n subintervalos de valor Δx = (b-a)/n. Em seguida escolhemos, aleatoriamente, um ponto xi* e calculamos a soma de f(xi*)Δx. Quando n tende ao infinito, o valor da aproximação feita pelo método das somas de Riemann tende ao valor exato da integral definida.

![Descrição da imagem]([https://upload.wikimedia.org/wikipedia/commons/thumb/2/2d/Riemann_sum_example.png/640px-Riemann_sum_example.png](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwp.ufpel.edu.br%2Fbottega%2Ffiles%2F2015%2F02%2FapostilaC22015.pdf&psig=AOvVaw0u0YDU8VEto_U9OAj7wBFI&ust=1757899960514000&source=images&cd=vfe&opi=89978449&ved=0CBUQjRxqFwoTCICXrO6N148DFQAAAAAdAAAAABAL))

desde que o limite exista e dê o mesmo valor para todas as possíveis escolhas de pontos xi*. Se ele existir, dizemos que f é integrável em [a, b].

Podemos observar graficamente esse conceito pelo meio dos n retângulos criados durante as subdivisões explicitadas anteriormente:

![Exemplo gráfico da soma de Riemann](https://i.imgur.com/5iQyxLZ.png)

Quanto mais aumentamos o número de subintervalos, ou seja, o Δx (que representa o valor da base desses retângulos) diminui, melhor se aproxima o valor da soma das áreas dos retângulos da área real (valor representado na cor rosa da figura abaixo).
