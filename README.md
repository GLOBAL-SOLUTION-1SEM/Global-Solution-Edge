Link da simulação: https://wokwi.com/projects/399321327390121985

## Contato

Bruno Biletsky  - RM: 554739
Enrico Ricarte  - RM: 558571
Victor Freire   - RM: 556191

# Projeto global solution (oceano) - BitWise

Nosso projeto foi feito com base na necessidade de monitorar as condições dos oceanos, possibilitando sua preservação e consequentemente a boa manutenção de todo seu ecossistema.
## Descrição

Este código é projetado para monitorar e exibir informações sobre temperatura e luminosidade utilizando um Arduino e componentes periféricos como um sensor DHT22 (para temperatura), um sensor de luminosidade e um display LCD.

- Ele inicializa os pinos necessários para conexão dos componentes.
- Inicializa o display LCD para exibir as informações.
- Lê os dados do sensor de temperatura DHT22 e calcula uma média móvel para suavizar as leituras.
- Lê os dados do sensor de luminosidade e também calcula uma média móvel.
- Com base nas leituras, determina o status da temperatura e período de pesca.
- Atualiza o display LCD para mostrar as informações relevantes, alternando entre as seções a partir de um botão. Entende-se por seções a exibição da temperatura, luminosidade e período de pesca.
- Controla LEDs para indicar o status atual das condições ambientais e de pesca: verde para adequado, amarelo para condições intermediárias e vermelho para condições críticas (incluindo proibições).
- Utiliza o módulo RTC (Real-Time Clock) para obter e exibir a data e hora atuais, além de verificar períodos específicos em que a pesca é proibida.

Este código permite o monitoramento constantemente das condições ambientais e de pesca essenciais para preservar o oceano e seu ecossistema.

## Funcionalidades Principais

1. **Monitoramento de Temperatura**: O código lê os dados do sensor DHT22 para medir a temperatura do ambiente. Ele calcula uma média móvel para suavizar as leituras e determinar o status desses parâmetros.
2. **Monitoramento de Luminosidade**: Utilizando um sensor de luminosidade, o código monitora os níveis de luz ambiente. Para temperatura, é calculada uma média móvel para suavizar as leituras.
3. **Exibição de Informações no Display LCD**: A partir de um botão pode-se alterar entre as seções de informações no display LCD, exibindo temperatura, luminosidade e período de pesca.
4. **Indicação Visual do Status Ambiental e possibilidade de pesca**: Com base nas leituras dos sensores, o código controla LEDs para indicar o status das condições ambientais e de pesca. Os LEDs acendem em verde para condições adequadas e pesca permitida, amarelo para condições intermediárias e vermelho para condições críticas e pesca proibida.
5. **Atualização Contínua das Informações**: Antes de refletir a leitura dos sensores no display LCD e nos indicadores visuais, as leituras passam por um processo de média móvel. Essa técnica permite uma maior estabilidade e confiabilidade nas leituras, suavizando possíveis variações abruptas e fornecendo uma representação mais precisa das condições ambientais ao longo do tempo. Essa abordagem aumenta a precisão do monitoramento, fornecendo informações mais consistentes para tomadas de decisão na gestão da preservação dos oceanos e seu ecossistema.

## Instalação

As instalações (hardware) necessárias para o código fornecido incluem:

1. **Sensor DHT22**: Este sensor é utilizado para medir a temperatura do ambiente.
2. **Módulo sensor fotoresistor (LDR)**: Um sensor de luminosidade é empregado para medir os níveis de luz ambiente.
3. **Display LCD1602 I2C**: Um display LCD é usado para exibir as informações sobre temperatura e luminosidade.
4. **LEDs**: LEDs são utilizados para indicar visualmente o status das condições ambientais e de pesca. Normalmente, são empregadas três cores diferentes de LEDs: verde para condições adequadas e/ou pesca permitida, amarelo para condições intermediárias e vermelho para condições críticas e/ou para pesca proibida.
5. **Arduino Board**: O código é projetado para ser executado em uma placa Arduino, que serve como a unidade de processamento principal.
6. **Conexões e Componentes Eletrônicos**: Além dos componentes mencionados acima, podem ser necessários resistores, fios, jumpers e outros componentes eletrônicos para realizar as conexões entre os sensores, LEDs, buzzer, display LCD e a placa Arduino.

Certifique-se de conectar corretamente os componentes à placa Arduino conforme especificado na simulação.

## Como Usar

O código fornecido é útil quando você precisa monitorar e controlar as condições ambientais, como temperatura, luminosidade e o período de pesca (com data em tempo real) nas águas dos oceanos e mares.
