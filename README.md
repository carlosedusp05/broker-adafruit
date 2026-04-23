# broker-adafruit
## Dashboard de Temperatura e Umidade com ESP32 e Adafruit IO - Projeto Didático IIoT

Este projeto foi desenvolvido como parte das atividades práticas do curso de **IIoT (Internet das Coisas Industrial)** no **SENAI**. O objetivo principal é coletar dados ambientais de temperatura e umidade em tempo real e transmiti-los via protocolo **MQTT** para a plataforma de nuvem **Adafruit IO**, permitindo o monitoramento remoto através de um dashboard intuitivo.

## Descrição do Projeto

O sistema utiliza um sensor **DHT11** acoplado ao **ESP32** para realizar a leitura das variáveis climáticas. O microcontrolador conecta-se à rede Wi-Fi e atua como um cliente MQTT, publicando os dados em "feeds" específicos no broker da Adafruit. 

Esta aplicação simula cenários industriais reais onde o monitoramento de condições ambientais é crítico, como em servidores (data centers), estoques de insumos sensíveis ou estufas automatizadas.

## Recursos e Componentes

Para a montagem deste esquema, foram utilizados os seguintes itens:

* **Microcontrolador:** ESP32 (Espressif Systems)
* **Sensor:** DHT11 (Temperatura e Umidade)
* **Conexão:** Protoboard e Jumpers (Macho-Fêmea / Macho-Macho)
* **Alimentação/Dados:** Cabo Micro-USB
* **Plataforma Cloud:** Adafruit IO (Broker MQTT)
* **Protocolo de Comunicação:** MQTT

## Bibliotecas (Library Manager)
Instale as seguintes bibliotecas através do Gerenciador de Bibliotecas (`Ferramentas` -> `Gerenciar Bibliotecas...`):

* **DHT sensor library** (Adafruit): Para comunicação com o sensor DHT11.
* **Adafruit Unified Sensor**: Dependência básica necessária para sensores Adafruit.
* **Adafruit MQTT Library**: Biblioteca principal para realizar a conexão e publicação no broker da Adafruit IO.

## Funcionalidades

* Leitura precisa de temperatura e umidade.
* Conexão automática com rede Wi-Fi.
* Publicação de dados em intervalos regulares para a nuvem via protocolo MQTT.
* Visualização de gráficos e indicadores em tempo real via dashboard web/mobile no Adafruit IO.

## Autores

* [Carlos Eduardo](https://github.com/carlosedusp05)
