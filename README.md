# Projeto: Utilização Inicial dos GPIOs com STM32F411

Este projeto demonstra a utilização básica dos GPIOs (General Purpose Input/Output) em um microcontrolador STM32F411. Um LED será configurado para piscar em uma frequência fixa e, após apertar um botão, a frequência de piscagem será aumentada.

## Requisitos de Hardware

- Microcontrolador STM32F411
- LED (conectado a um pino GPIO)
- Botão (conectado a um pino GPIO)
- Resistor de pull-up/pull-down para o botão (se necessário)
- Fonte de alimentação adequada
- Placa de desenvolvimento (por exemplo, STM32 Nucleo-F411RE)

## Ferramentas de Software

- STM32CubeMX
- IDE (Integrated Development Environment) como STM32CubeIDE
- Biblioteca HAL (Hardware Abstraction Layer) da STMicroelectronics

## Configuração de Hardware

1. Conecte o LED a um pino GPIO de saída P13
2. Conecte o botão a um pino GPIO de entrada PA0

![image](https://github.com/MatKenji/GPIO_Led_Blink_Switch/assets/169562589/1ce414b3-1622-4087-9b58-b4cec2a74858)

3. Configure resistores pull-UP para o botão.

![image](https://github.com/MatKenji/GPIO_Led_Blink_Switch/assets/169562589/233a5b29-d78d-4b80-bab7-e4aadd0dee89)

4. Configure o botão output HIGH e maximum output speed Low

![image](https://github.com/MatKenji/GPIO_Led_Blink_Switch/assets/169562589/f45a3540-46cf-40c6-a087-31f017c222fb)

## Resultados

1. Após configurar o microcontrolador e o software conforme descrito no README, o LED deve começar a piscar quando o sistema é ligado.

2. Ao pressionar o botão, a frequência de piscagem do LED deve aumentar, permitindo uma visualização clara da resposta do sistema ao evento de pressionamento do botão.
Considerações

3. A implementação de um debounce simples no software ajuda a garantir que o sistema responda apenas às mudanças de estado reais do botão, ignorando ruídos ou flutuações de curto prazo.

4. Aumentar a frequência de piscagem do LED pode resultar em um consumo de energia mais alto. Isso é importante considerar em aplicações alimentadas por bateria ou com restrições de energia.

**Nota:** Os arquivos de código fornecidos neste repositório foram desenvolvidos usando STM32CubeIDE. Devido a limitações de minha experiência com o STM32CubeIDE, a importação direta do projeto para o Git pode não ter sido feita da maneira mais eficiente ou padronizada. 
