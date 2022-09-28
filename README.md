# STM32F103_UART_TIMER
Using the UART to print to a PC's serial port.

Neste exemplo, o STM32F103C8T6 (Bluepill) é usado para enviar informações via UART.
A informação enviada é o tempo gasto para se realizar em envio de 6 bytes usando a função HAL_UART_Transmit(huart, pData, Size, Timeout);

Para conectar o STM32F103 com o PC foi usado um módulo conversor USB-TTL CH340, igual ao mostrado na figura abaixo:

![UART_Ch340](https://user-images.githubusercontent.com/114233216/192904439-a17834ad-36cb-405e-8c37-ce8bd758f2d1.jpg)

Para usar esse conversor é preciso instalar um drive, que pode ser encontrado no link: https://sparks.gogo.co.nz/ch340.html

A Conexão entre o módulo conversor e o STM32 é mostrado no esquema abaixo:

![conversor usb ttl - stm32](https://user-images.githubusercontent.com/114233216/192904499-e98ba9db-8d90-4cb8-bec3-49f3a030ca9f.png)


O software usado como Terminal Serial foi o TERMITE. É um software gratuito facilmente encontrado para download no Google.

1. Configuração do Clock
![UART_Clock](https://user-images.githubusercontent.com/114233216/192904809-abc366b4-120f-45dc-aaf0-a52b7cdfe089.png)


3. Configuração do USART
![UART_uart](https://user-images.githubusercontent.com/114233216/192904823-b12a101c-0452-4ff7-8bb3-850682ba80e0.png)

4. Configuração do TIMER 2
![UART_tim2](https://user-images.githubusercontent.com/114233216/192904863-be20f6c0-f491-40b2-92b8-bd1ababe0be0.png)


5. Configuração do GPIO
![UART_gpio](https://user-images.githubusercontent.com/114233216/192904830-b7fb151b-4dd7-4b0d-8de1-5be55bed48dc.png)


6. Principal parte do Código
![UART_code2](https://user-images.githubusercontent.com/114233216/192904898-d26d5ceb-5a60-4793-ae3e-5ca14a7e374c.png)

O Código completo está localizado em Src>Main.c



