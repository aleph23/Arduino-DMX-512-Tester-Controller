**Hardware**

**Notas sobre la versión**

***

**vx.x - Beta - Firm vx.x**
- AGREGADO  - Adafruit HXD8357D - 3.5" TFT 320x480 + Touchscreen Breakout Board w/MicroSD Socket
			- https://learn.adafruit.com/adafruit-3-5-color-320x480-tft-touchscreen-breakout/overview
- AGREGADO  - Adafruit STMPE610 - Resistive Touch Screen Controller
			- https://www.adafruit.com/products/1571
			
***

**v0.7 - Beta - Firm v1.7**
- AGREGADO   - SW para Key Light
- AGREGADO   - SW para Ext Light
- AGREGADO   - Espaciadores para fijacion
- AGREGADO   - Leyendas de conexion

***
 
**v0.6 - Beta - Firm v1.7**
- AGREGADO   - regulador para fuente externa, el arduino se calienta
- AGREGADO   - bornera para salida de fuente regulada de 5V para uso general
- AGREGADO   - led para salida de fuente regulada
- AGREGADO   - boton de reset
- AGREGADO   - opto acoplado a salida de dmx
- AGREGADO   - convertidor de DC/DC para asilamiento de DMX
- AGREGADO   - SW de palanca para invertir polaridad de salida de DMX
- AGREGADO   - Al encoder capacitores para rebote
- AGREGADO   - jumper default eeprom en pin 9
- AGREGADO   - driver para luz led como lampara
- AGREGADO   - capacitores al teclado para rebote
- AGREGADO   - logo de Open Hardware
- CORREGIDO  - se eliminan los cursores, los remplaza el encoder
- CORREGIDO  - se saco el encoder de la placa original y se solda directo a la placa
- CORREGIDO  - se elimina el data I/O
- CORREGIGO  - se quito la entrada al Arduino desde el MAX485, causa problemas al cargar el programa
- CORREGIDO  - Las bases de los CI se cambiaron a maquinadas
- Optoacoplamiento basado en http://www.mathertel.de/Arduino/DMXShield.aspx
- CHECAR     - en firmware que el encoder DT y CLK que sean pullup

***

**v0.5 - Beta - Firm v1.6 to 1.7**
- CORREGIDO - potenciómetro por encoder
- CORREGIDO - etapa de potencia para contraste
- AGREGADO 	- Luz para el teclado y cursores
- AGREGADO  - Etapa de potencia para luz de teclado
- Contraste por PWM basado en http://www.pcbheaven.com/circuitpages/PWM_LCD_Contrast_Control/

***

**v0.4 - Beta - Firm v0.9 to v1.3**
- CORREGIDO - hacer más grandes los pads del SW
- CORREGIDO - quitar parte de abajo del soporte del teclado estorba con el flex del teclado
- CORREGIDO - recorrida la bornera de la conexión dmx hacia el arduino, queda más centrada
- CORREGIDO - acercar la base del mx485 al borde de la placa para que el teclado no estorbe
- CORREGIDO - agregar un diodo rectificador a la entrada de la batería
- CORREGIDO - se hizo más chico el puente que estaba dentro del área del arduino
- CORREGIDO - los datos de la salida están al revés
- AGREGADO  - interconectados los pines del arduino de vcc y gnd faltantes
- AGREGADO  - la leyenda open hardware a bottom

***

**v0.3 - Beta - Firm v0.9 to v1.3**
- AGREGADO  - backlight a pin 13 para efecto en el lcd mientras se actualiza
- AGREGADO  - control de contraste desde software
- AGREGADO  - control de back light desde software
- CORREGIR  - agregar capacitores al backlight y al contraste, parpadea con baja frecuencia
- CORREGIR  - acercar el potenciómetro a los pads y marcar el pad del centro
- CORREGIR  - acercar la base del mx485 al borde de la placa para que el teclado no estorbe
- CORREGIR  - la placa del teclado tiene mal ubicado el header de abajo donde pasa el flex del teclado
- CORREGIR  - agregar un diodo rectificador a la entrada de la batería
- CORREGIR  - agregar serigrafía a top en el pcb
- CORREGIR  - hacer más grandes los pads del SW
- CORREGIR  - quitar parte de abajo del soporte del teclado estorba con el flex del teclado
- CORREGIR  - los datos de la salida están al revés

***

**v0.2 - Beta - Firm v0.0 to v0.8**
- AGREGADO  - control de contraste desde software
- AGREGADO  - control de back light desde software

***

**v0.1 - Beta - Firm v0.0 to v0.8**
- CORREGIDO - no se necesita el led on, la pantalla ya tiene un led
	    - el led ON se retira, los leds de la salida del dmx indican que está activo
- CORREGIDO - no hay botón de reset
	    - no se requiere el botón de reset, hay un switch de on off
- CORREGIDO - quitar botón SW de encendido
	    - se cambió por un switch deslizable
- CORREGIDO - base de teclado, darle más soporte
	    - no requiere más soporte
- CORREGIDO - eliminar la fuente de alimentacion regulada
	    - se eliminó la fuente regulada
- CORREGIDO - quitar de los conectores USB y power del arduino, las conexiones de arriba, no permiten que cierre bien el arduino
	    - se reubicaron los componentes
- CORREGIDO - pasar los conectores a la parte de abajo, pesa mucho la placa
	    - los conectores se pasaron a la parte de abajo
- CORREGIDO - agregar capacitores cerámicos a los botones para el rebote
	    - agregados, cerámicos 104, mejoro la estabilidad en la lectura
- CORREGIDO - se cambió el conector XLR de 3 pin por conector amphenol de 3 y 5 pin, son más resistentes
- CORREGIDO - los leds de la salida del DMX se cambiaron a la parte de abajo y viendo hacia abajo, molestaba a la vista
- CORREGIDO - el pcb se redujo
- AGREGADO  - etapa de potencia para controlar el back light del LCD
- AGREGADO  - conexión para baterías
- AGREGADO  - header para completar la conexión del arduino, estaba incompleta

***

**v0.0 - Beta - Firm v0.0 to v0.8**
- CORREGIR  - no se necesita el led on, la pantalla ya tiene un led
- CORREGIR  - no hay botón de reset
- CORREGIR  - quitar botón SW de encendido
- CORREGIR  - agregar canon XLR de 5 pin
- CORREGIR  - base de teclado, darle más soporte
- CORREGIR  - eliminar la fuente de alimentacion regulada, arduino ya tiene una fuente regulada
- CORREGIR  - quitar de los conectores USB y power del arduino, las conexiones de arriba, no permiten que cierre bien el arduino
- CORREGIR  - pasar los conectores a la parte de abajo, pesa mucho la placa
- CORREGIR  - agregar capacitores cerámicos a los botones para el rebote