# Fonte de tensão ajustável (3V-12V)

A fonte de tensão é um circuito que transforma a corrente alternada para continua com os parametros de uma corrente efetiva de 100mA e voltagem variando de 3V até 12V.

## Componentes

### Transformador

O transformador é a parte inicial do circuito. Ele, neste circuito, é resposavel por diminuir a tensão que recebemos da tomada para um valor que possamos trabalhar com.
Sabendo que, em teoria, a tensão RMS (root mean square) no Brasil é 127V temos:

$RMS = \frac{Vpico}{\sqrt{2}}$

$127V = \frac{Vpico}{\sqrt{2}}$

$Vpico = 127 \cdot \sqrt{2} \approx 179.605$

Durante as aulas medimos a tensão dos transformadores, obtendo para o utilizado uma tensão de aproximadamente 24.2V.
Sabendo que a proporção de espiras é dado por:

$Prop = \frac{VpicoAntes}{VpicoDepois}$

$Prop = \frac{179.6}{24.2} \approx 7.42$

Dessa forma obtendo as especificações do transformador utilizado.

### Ponte retificadora completa

A ponte retificadora completa é uma configuração de 4 diodos que utilizamos para direcionar a tensão vinda do transformador para um unica direção do circuito.

O circuito sem a ponte funcionaria polarizado de duas formas por um periodo a tensão vai na direção "positiva" e outra na "negativa".

<img src="./imgs/lowgifAC.gif">

Agora quando usamos a ponte retificadora temos que independente da direção da corrente alternada ela sempre caminhara pelo caminho que desejamos. Pois quando positivo, a tensão vem da parte de cima, o diodo da esquerda inibe que ele va pela esquerda e direciona para a direita, quando negativo, a tensão vem pela parte de baixo sobre a mesma lógica.

<img src="./imgs/lowgifDC.gif">

É notavel que na ponte retificadora completa existe uma queda de tensão pois um diodo de sicilio dissipa uma tensão de aproximadamente 0.7V.

Eu escolhi uma ponte retifacdora ja pré preparada com o nome Ponte Retificadora 2W10 pois era a mais conveniente de se colocar no circuito.

### Capacitor 

O capacitor é o componente responsavel por

## Custo dos componentes

| Componente               | Preço   |
|--------------------------|---------|
| Ponte Retificadora 2W10  | R$ 1.10 |
| Capacitor de 470uF/25V   | R$ 0.65 |
| 2*Resistor de 2K2        | R$ 0.16 |
| LED verde                | R$ 0.50 |
| 2*Resitor de 510R (1/4)W | R$ 0.14 | 
| Diodo Zener 13V (1/2)W   | R$ 0.70 |
| Potenciômetro 10k linear | R$ 7.00 |
| Resistor de 1k (1/4)W    | R$ 0.07 |
| Resitor de 120R 5W       | R$ 1.40 |
| BC548B                   | R$ 0.30 |

Total = R$ 14.16

Obs: Preço considerando o valor unitario de cada um dos componentes

## Circuito no Falstad

<a href="https://tinyurl.com/2pcby8al"><img src="./imgs/CircuitoFalstad2.jpg">

Link para o circuito: https://tinyurl.com/2pcby8al

## Circuito Montado

Uma imagem do circuito de uma visão por cima:

<img src="./imgs/CircuitoCima.jpg">

Imagens do circuito com uma resistencia de 120Ohms como teste:

<img src="./imgs/CicuitoPotBaixo.jpg">

<img src="./imgs/CircuitoPotCima.jpg">

## Esquemático da PCB no EAGLE

## PCB no EAGLE

## Feito por:

Vinícius Souza Freitas - 15491959

## Agradecimentos

Profesor Simões, que encotrou o problema quase instantaneamente enquanto eu e o kaita ficamos umas 3 horas tentando encontra-lo.

Jonas Kaita, um dos maiores cozinheiros.
