# Sensor de Proximidade (PIR) + LED

**Discente:** Erik Felipe de Andrade Dalonso  
**Docente:** Amanda Paul Dull

Este repositório contém a atividade prática de IoT utilizando um Arduino UNO, um sensor de movimento PIR e um LED.

## 🔗 Simulação
(https://www.tinkercad.com/things/6eHG3DZ7fHJ-pir-led)


## Enunciado: Sensor PIR + LED

A atividade consiste em utilizar um sensor de movimento PIR para acionar um LED automaticamente ao detectar presença ou movimento no ambiente.

Quando o sensor PIR detecta movimento, o pino de saída envia um sinal ao Arduino, que aciona o LED. Quando o movimento cessa, o LED é desligado.

## Materiais necessários

| Qtd | Componente |
| --- | --- |
| 1 | Placa Arduino UNO |
| 1 | Cabo USB |
| 1 | Protoboard |
| 1 | Sensor de Movimento PIR |
| 1 | LED azul difuso de 5 mm |
| 1 | Resistor de 220 Ω |
| — | Fios de jumper macho-macho |

## Como foi feita a atividade

A protoboard foi alimentada conectando os pinos 5V e GND do Arduino aos barramentos principal e superior de alimentação.

O sensor PIR foi conectado aos barramentos de alimentação (VCC e GND) e seu pino de sinal foi ligado à porta digital 7. O LED azul foi montado com um resistor de 220 Ω em série ligado ao GND, com seu anodo conectado à porta digital 2.

No programa, o Arduino faz a leitura do pino digital 7: ao detectar nível lógico alto vindo do sensor PIR, o código aciona a saída digital 2 para acender o LED, desligando-o quando nenhum movimento for detectado.
