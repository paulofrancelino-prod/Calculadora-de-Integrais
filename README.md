# 📐 Calculadora de Integrais com Soma de Riemann  

Este projeto tem como objetivo **calcular o valor aproximado de integrais definidas** a partir de uma função e de um intervalo dados pelo usuário. O cálculo é feito utilizando o método da **Soma de Riemann**, com margem de erro ajustável.  

---

## 📌 Introdução  

A integral definida pode ser interpretada como a **área sob a curva** de uma função \( f(x) \).  
Para aproximar esse valor, existem diversos métodos numéricos, sendo a **Soma de Riemann** um dos mais clássicos e didáticos.  

Neste projeto em Python, implementamos esse conceito para obter aproximações numéricas com uma margem de erro configurável (neste caso, 10e-6)

---

## 📖 Conceito Teórico  

Temos a ideia geral da integral definida, com base no livro de James Stewart, como sendo a seguinte: Dada uma função f contínua definida em a ≤ x ≤ b de intervalo, dividimos o intervalo [a, b] em n subintervalos de valor Δx = (b-a)/n. Em seguida escolhemos, aleatoriamente, um ponto xi* e calculamos a soma de f(xi*)Δx. Quando n tende ao infinito, o valor da aproximação feita pelo método das somas de Riemann tende ao valor exato da integral definida. Desde que o limite exista e dê o mesmo valor para todas as possíveis escolhas de pontos xi*. Se ele existir, dizemos que f é integrável em [a, b]. Quanto mais aumentamos o número de subintervalos, ou seja, o Δx (que representa o valor da base desses retângulos) diminui, melhor se aproxima o valor da soma das áreas dos retângulos da área real (valor representado na cor rosa da figura abaixo).

## ⚙️ Como o Código Funciona?  

O código:  
- Recebe a função \( f(x) \) como **input** do usuário.  
- Solicita os limites de integração \( a \) e \( b \).  
- Define uma **margem de erro** para a aproximação.  
- Calcula a soma de Riemann com subdivisões sucessivas até alcançar o erro especificado.  

---

## ▶️ Como Usar?  

1. Rode o código no seu ambiente Python (ou no [Google Colab](https://colab.research.google.com/)).  
2. Insira:  
   - A função \( f(x) \)  
   - O limite inferior \( a \)  
   - O limite superior \( b \)  
   - A margem de erro desejada  
3. Aguarde o resultado:  
   - O valor aproximado da integral  
   - O número de subdivisões utilizadas  

---

## 📊 Exemplo de Uso  

Entrada:  
```python
f(x) = x**2
a = 0
b = 1
erro = 1e-6
