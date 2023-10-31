# BCC-UERN-TCC
Repositório destinado ao versionamento da implementação lógica do Robô que dará origem ao TCC da Gradução em CC. 

Foram utilizados até o momento (26/06/2022):

 - 1 Arduino Uno – placa de microcontrolador baseado no ATmega328, com 14 pinos de entradas/saídas digitais, 6 entradas analógicas e conexão USB;
 - 5 Matriz de LEDs 8×8 com [driver MAX7219](http://pdfserv.maximintegrated.com/en/ds/MAX7219-MAX7221.pdf);
 - Jumpers fêmea-fêmea;
 - Jumpers macho-fêmea;
 - 1 computador (para compilar e fazer o upload do código para o Arduino);

Programação feita na IDE Arduino 1.8.19, onde foi necessário adicionar a biblioteca [LedControl.h](https://github.com/wayoda/LedControl)



---
Orientações Gerais :)

---


# Python

Criei e ative o ambiente virtual:

Criar:
```
virtualenv .vozes 
```


Ativar:
```
.\.vozes\Scripts\activate    
```

Instale os "requirements.txt"

```
pip install -r requirements.txt
```

As vozes só serão executadas mediante comunicação serial com o arduino. Portanto, ao conectar o arduino ao computador, imediatamente, a aplicação python deve ser executada.

Caso a aplicação python seja executada antes de conectar a aplicação será gerado um erro na comunicação da serial port.

caso seja conectado muito tempo após a conexão da aplicação python, será gerado uma execução não sincronizada das falas.

Portanto, após conectar a aplicação arduino, o tempo máximo para iniciar a aplicação python é de no máximo 10s.

# Arduino
Primeiro envie o código arduino para a placa;

Em seguinda execute (imediatamente) o código python.



