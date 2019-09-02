# ATENUADORES
Em projetos que envolvem diferentes níveis de tensão em forma de blocos encadeados, de forma geral, necessitam de atenuação de um bloco para outro, obedecendo a especificações tais como de figura de ruído e potência, por exemplo.

### 1.ATENUADORES DIGITAIS
A fim de possibilitar um controle via software, os atenuadores digitais são preteridos no lugar de atenuadores fixos. Em sistemas de comunicações, esses elementos são responsáveis pelo controle automático de ganho em rádios definidos por software, por exemplo.
Abaixo é possível observar o diagrama de blocos interno ao chip HMC542BLP4E:

![HMC542BLP4E Diagrama de Blocos Interno](https://github.com/apct-2019/Mendes/blob/master/atenuador1.JPG)

### 2.CARACTERÍSTICAS
As características básicas do HMC542BLP4E são as listadas abaixo:

#### Componente: HMC542BLP4E
#### Tensão de Alimentação: 5v
#### Corrente de Alimentação: 2.8mA
#### Atenuações possíveis: 0.5,1,2,4,8 e 16dB (máximo de 31.5dB)
#### Faixa de Frequências: DC a 4GHz
#### Perda de inserção: 1.7dB
#### Potência de entrada (para 0.1 dB de Compressão): 30dBm (Típico)
#### Precisão: 0.25dB
#### Dimensões: 4x4mm
#### Package: QFN-24

Nesse tipo de componente, é muito importante notar que para haver uma atenuação de tal forma que não distorça o sinal, ou seja, mantenha o sinal, a menos da amplitude, não pode haver uma compressão de sinal grande (acima de 1dB). O fabricante garante que a 0.1 dB de compressão a potência de entrada recomendada é cerca de 30dBm, portanto sem haver distorções na saída. No campo das atenuações possíveis, o cálculo se dá pela soma simples dos valores que se deseja adicionar à atenuação, sendo que, tendo selecionado todos os valores no registrador correspondente, o máximo valor corresponde a 31.5dB.

### 3.COMUNICAÇÃO
A comunicação com o ci é feita a partir do protocolo SPI, com visualização simplificada nos esquemáticos abaixo.

Fisicamente, a atenuação pode ser entendida como mostrada a seguir. Observe no bloco as diversas possibilidades de atenuação presentes no diagrama do componente.
![Comunicação SPI com o Atenuador](https://github.com/apct-2019/Mendes/blob/master/atenuador3.JPG)

O padrão da comunicação segue o informado na imagem:
![Comunicação SPI com o Atenuador](https://github.com/apct-2019/Mendes/blob/master/atenuador5.JPG)

### 3.Circuito
O circuito a seguir é o recomendado pelo fabricante:
![Circuito Proposto](https://github.com/apct-2019/Mendes/blob/master/atenuador4.JPG)

### 4.DATASHEET
O manual do componente escolhido pode ser encontrado no link: https://www.analog.com/media/en/technical-documentation/data-sheets/hmc542b.pdf
