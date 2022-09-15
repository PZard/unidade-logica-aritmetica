# Unidade Lógica e Aritmética

Projeto desenvolvido para a disciplina de Fundamentos de Sistemas Computacionais.

Acadêmicos:

- Pedro Zardin Guimarães
- Enzo Augusto Tonatto


Construção da ULA:

Primeiramente foi construído dois registradores de deslocamento de 8 bits, nos quais o armazenador A ficará responsável por guardar o primeiro operando e exibir o resultado após o processo, enquanto armazenador B apenas guardará o segundo operando.  

<img src="/img/Registrador.png"><img>

Após isso criamos o multiplexador de 4 entradas (MUX 4x1), que é responsável por colocar sequencialmente várias informações paralelas. 

<img src="/img/Multiplexador.png"><img>

Depois foi adicionado o circuito somador completo (Full Adder) que é representado por três entradas, A, B e Carry In, que são somados e obtemos o resultado da soma, ou sinal Sum de saída, e Carry out. 

<img src="/img/Full Adder.png"><img>

Foram adicionados também uma porta AND, uma porta OR e duas portas XOR. 

<img src="/img/Componentes Combinacionais Básicos.png"><img>

Em seguida começamos a montar nossa Unidade Lógica Aritmética ligando os componentes combinacionais básicos ao multiplexador e ao somador completo. Também foi adicionado um clock e um flip-flop para a propagação de carry. 

<img src="/img/Adição de Multiplexador, Full Adder e Flip Flop tipo D.png"><img>

Por fim finalizamos nossa Unidade Lógica Aritmética adicionando os registradores, feitos inicialmente, e dois displays (HEX displays) associados aos registradores com o objetivo de apresentar os valores de forma visual.  

<img src="/img/Adição de Registradores e Displays.png"><img> 
