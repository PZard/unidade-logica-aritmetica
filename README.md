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

Operações:

ADD – Para a soma de dois valores é necessário, primeiramente, adicionar os valores nos registradores A e B, após isso selecionar o valor 1 1 no seletor de operação, com isso o MUX estará configurado para a quarta porta que é alusivo a operação de adição. Sendo assim, serão necessários oito pulsos de clock para o obter o resultado. 

<img src="/img/add1.png"><img> 

Resultado:

<img src="/img/add2.png"><img> 

SUB – Para realizar uma subtração, precisamos de dois valores nos registradores A e B e definir o valor 1 1 no seletor de operação, assim como fizemos na adição, porém para a subtração acontecer devemos inverter o operando B, sendo assim ligamos o Binvert em nossa ULA e adicionamos o valor de 1 para o carry. Após isso, pulsamos o clock oito vez.  

<img src="/img/sub1.png"><img>

Resultado:

<img src="/img/sub2.png"><img> 

AND – Para a utilização da porta AND é preciso os valores de ambos os registradores estejam escolhidos e que o seletor de operação esteja definido em 0 0, referenciando-se a primeira porta. Depois são necessários os oito pulsos de clock, para receber o resultado.  

<img src="/img/and1.png"><img>

Resultado:

<img src="/img/and2.png"><img>

OR - Para a utilização da porta AND é preciso os valores de ambos os registradores estejam escolhidos e que o seletor de operação esteja definido em 0 1, referenciando-se a segunda porta. Depois são necessários os oito pulsos de clock. 

<img src="/img/or1.png"><img>

Resultado:

<img src="/img/or2.png"><img>

XOR - Para a utilização da porta XOR é preciso os valores de ambos os registradores estejam escolhidos e que o seletor de operação esteja definido em 1 0, referenciando-se a terceira porta. Depois são necessários os oito pulsos de clock.  

<img src="/img/xor1.png"><img>

Resultado:

<img src="/img/xor2.png"><img>

NOT – Para fazer um NOT precisamos definir um valor no operando B e este valor será quem será negado, já no operando A devemos definir o valor 1111 1111, após isso selecionar a porta referente ao XOR no MUX, ou seja, o valor 1 0 no seletor de operações e por fim os oitos pulsos de clock para obter o valor negado.  

<img src="/img/not1.png"><img>

Resultado:

<img src="/img/not2.png"><img>
