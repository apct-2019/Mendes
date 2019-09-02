# ATENUADORES
Em projetos que envolvem diferentes níveis de tensão em forma de blocos encadeados, de forma geral, necessitam de atenuação de um bloco para outro, obedecendo a especificações tais como de figura de ruído e potência, por exemplo.

### 1.ATENUADORES DIGITAIS
A fim de possibilitar um controle via software, os atenuadores digitais são preteridos no lugar de atenuadores fixos. Em sistemas de comunicações, esses elementos são responsãveis pelo controle automático de ganho em rádios definidos por software, por exemplo.
Abaixo é possível observar o diagrama de blocos interno ao chip HMC542BLP4E:

![HMC542BLP4E Diagrama de Blocos Interno](https://github.com/apct-2019/Mendes/blob/master/atenuador1.JPG)

### 2.CARACTERÍSTICAS
As características básicas do HMC542BLP4E são as listadas abaixo:

#### Componente: HMC542BLP4E
#### Tensão de Alimentação: 5v
#### Corrente de Alimentação: 2.8mA (Cada)
#### Dimensões: 4x4mm
#### Package: QFN-24

### 3.COMUNICAÇÃO
A comunicação com o ci é feita a partir do protocolo SPI, com visualização simplificada nos esquemáticos abaixo.

Fisicamente, a atenuação pode ser entendida como mostrada a seguir:
![Comunicação SPI com o Atenuador](https://github.com/apct-2019/Mendes/blob/master/atenuador3.JPG)

O padrão da comunicação segue o informado na imagem:
![Comunicação SPI com o Atenuador](https://github.com/apct-2019/Mendes/blob/master/atenuador2.JPG)

### 3.Circuito
O circuito a seguir é o recomendado pelo fabricante:
![Circuito Proposto](https://github.com/apct-2019/Mendes/blob/master/atenuador4.JPG)

### 4.DATASHEET
O manual do componente escolhido pode ser encontrado no link: https://www.analog.com/media/en/technical-documentation/data-sheets/hmc542b.pdf
