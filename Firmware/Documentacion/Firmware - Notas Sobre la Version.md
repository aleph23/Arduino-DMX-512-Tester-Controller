**Firmware**

**Notas sobre la versión**

**Compilado en Arduino IDE v1.0.6**

***

**v0.x - Beta**
- AGREGAR - encoder
- AGREGAR - funcion para convertir a binario dip switch y viceversa
- AGREGAR - en multiplicador el valor en tiempo real desde el potenciometro o teclado
- AGREGAR - control chaser desde el potenciometro, al girar recorre los canales
- AGREGAR - dimmer para luz led como lampara

***

**v1.3 - Stable - Hardware v0.3 - v0.4**
- CORREGIR  - en control matrix cuando se selecciona un canal de la esquina el cursor parpadeando queda fuera de lugar
- AGREGADO  - Control de iluminacion para teclado
- AGREGADO  - a EEPROM la posicion 4092 para guardar key light
- AGREGADO  - la variable global int EEPROM_Limit para controlar el limite de escritura de eeprom de universos
- AGREGADO  - EEPROM_Limit a todas las funciones de memoria EEPROM
- AGREGADO  - el control * en el teclado controla el back light y el key light 
- AGREGADO  - variable global Light_On_Off para control desde tecla * de la iluminacion de teclado y back
- AGREGADO  - al about un dimmer en key y back durante el efecto binario
- AGREGADO  - a la tecla de light * un dimmer de on y off para key y back
- CORREGIDO - en Back_Light_En, byte Back_Light_Value = EEPROM.read(513); el valor esta fuera de rango
- CORREGIDO - unused variable 'EEPROM_Add'
- CORREGIDO - en about "open hardware!" por "Open Source License:"

***

**v1.2 - Stable - Hardware v0.3 - v0.4**
- AGREGADO  - al arranque toma el banco de la eeprom previamente elejido desde config
- AGREGADO  - a config el banco que lee a arranque
- AGREGADO  - al about el banco actual
- AGREGADO  - a about reacomodo de datos
- AGREGADO  - a about licencias open source
- AGREGADO  - a initial memory el bank actual
- AGREGADO  - en EEPROM add 4093 para guardar banco a correr al inicio
- AGREGADO  - Bank 8 solo tiene 509 canales disponibles
- AGREGADO  - a EEPROM Load el limite en bank 8 de 4092
- AGREGADO  - a EEPROM Save el limite en bank 8 de 4092
- CORREGIDO - GUI Config de LCD config solo a config
- CORREGIDO - GUI Config de Control a exit
- AGREGADO  - a GUI Config opcion bank init
- AGREGADO  - EEPROM_Load_Init para cargar el universo precnfigurado al inicio
- CORREGIDO - GUI about cambio de disposicion y url por wiki
- AGREGADO  - GUI_Licence a cofig

***

**v1.1 - Beta - Hardware v0.3 - v0.4**
- AGREGADO  - memory a control options
- AGREGADO  - a memory gui ClearAll para borrar todos los bancos de la eeprom
- AGREGADO  - a memory gui reacomodo de menues

***

**v1.0 - Beta - Hardware v0.3 - v0.4**
- CORREGIDO - seceuncer no tiene reversa
- CORREGIDO - secuencer no tiene salida de dmx, el uso de memoria eeprom descartaba valores
- CORREGIDO - GUI_Secuencer se cambió el método de lectura de memoria, se hace en tiempo real, evita over flow
- CORREGIDO - GUI_Secuencer se cambió a GUI_Control_Secuencer
- CORREGIDO - tabulacion
- CORREGIDO - manejo de memoria EEPROM al guardar y leer el conteo es en 1 y no en 0
- CORREGIDO - GUI_Chasser el cursor blink no se mostraba después de stop 
- CORREGIDO - GUI_Control_Options, el cursor no se mostraba en unitary
- CORREGIDO - disminucion de tiempo mensaje final de opciones de acceso a eeprom
- AGREGADO  - lectura de botón "center" en el about
- AGREGADO  - a GUI_Secuencer límite de delay a 100
- AGREGADO  - a GUI_Secuencer en la salida a control regresa al dmx los datos desde la ram
- AGREGADO  - a GUI_Unitary el canal anterior y siguiente en el gui

***

**v0.9 - Beta - Hardware v0.3 - v0.4**
- CORREGIR  - GUI_Secuencer provoca over flow y se reinicia, demasiada ram usada
- CORREGIDO - GUI_Navegar se cambió la variable Boton_Delay_Cursor de long a int
- CORREGIDO - Contrast_Init se limita a no menor de 150 el valor del pwm
- CORREGIDO - GUI_Config solo en control options
- CORREGIDO - esta encimado en control options unitary
- CORREGIDO - GUI Control Options se quitó iniciar:, no se usa
- CORREGIDO - se agregó variable global BackLight_Add para dirección de EEPROM
- CORREGIDO - se agregó variable global Contrast_Add para dirección de EEPROM
- CORREGIDO - Se quitó el efecto binario cuando se usa la memoria EEPROM
- AGREGADO  - GUI_Secuencer limitado delay entre 0 y 999 x 100 mS
- AGREGADO  - GUI_Secuencer limitado final y first entre 1 y 8
- AGREGADO  - a GUI_About bink del cursor
- AGREGADO  - GUI_Memory_Bank
- AGREGADO  - GUI_Memory_Bank, regresa 1 si se selecciona salir para regresar al menú anterior
- AGREGADO  - a GUI_Memory_Bank, retardo cuando entra al banco de memoria
- AGREGADO  - a matrix el número de banco actual, si el banco no se seleccionó muestra "-"
- AGREGADO  - a memory options el número de banco actual, si el banco no se seleccionó muestra "-"
- AGREGADO  - a unitary control el número de banco actual, si el banco no se seleccionó muestra "-"
- AGREGADO  - a multiply control el número de banco actual, si el banco no se seleccionó muestra "-"
- AGREGADO  - a GUI Memory la configuración
- AGREGADO  - a GUI Control Options el número de banco actual, si el banco no se seleccionó muestra "-"
- AGREGADO  - a GUI Control Options la configuración
- AGREGADO  - a GUI_EEPROM_Empty la leyenda del banco que se está modificando "RAM"
- AGREGADO  - a GUI_EEPROM_Empty el blink del lcd para saber que está trabajando
- AGREGADO  - a EEPROM_Clear control de universos guardados
- AGREGADO  - a EEPROM_Clear al final y al principio el número de banco
- AGREGADO  - a EEPROM_Clear el blink del lcd para saber que está trabajando
- AGREGADO  - a EEPROM_Clear regresa 1 si se selecciona éxito
- AGREGADO  - a EEPROM_Clear más tiempo para mensaje final
- AGREGADO  - a EEPROM_Load control de universos guardados
- AGREGADO  - a EEPROM_Load, regresa 1 si se selecciona exit
- AGREGADO  - a EEPROM_Load al final el número de banco
- AGREGADO  - a EEPROM_Load el blink del lcd para saber que está trabajando
- AGREGADO  - a EEPROM_Load más tiempo para mensaje final
- AGREGADO  - a EEPROM_Save control de universos guardados
- AGREGADO  - a EEPROM_Save al final el número de banco
- AGREGADO  - a EEPROM_Save, regresa 1 si se selecciona exit
- AGREGADO  - a EEPROM_Save el blink del lcd para saber que está trabajando
- AGREGADO  - a EEPROM_Save más tiempo para mensaje final
- AGREGADO  - a GUI_Memory_Init control de universos
- AGREGADO  - a GUI_Memory_Init manejo cuando se selecciona exit en los bancos de memoria
- AGREGADO  - a GUI_Memory control de salida desde bancos de memoria
- AGREGADO  - a GUI_Memory salida inmediata después de la lectura de opción
- AGREGADO  - a GUI_About la leyenda open hardware
- AGREGADO  - a GUI_About más tiempo para mostrar
- AGREGADO  - GUI Secuencer
- el banco 8 solo llegaría a 500 por el contraste y el backlight
- Los bancos de memoria no aplican a memory empty
- GUI_Memory_Bank solo actúa en cambios de EEPROM

***

**v0.8 - Stable - Hardware v0.3 - v0.4**
- compatibilidad con Hardware v0.3 - v0.4

***

**v0.7 - Stable - Hardware v0.0 - v0.2**
- AGREGADO  - en chaser el cursor en blink cuando hace la secuencia
- AGREGADO  - función de Black Out desde el menú de Memory, pone todos los canales en 0 y los regresa a lo que tenían, para salir dar en center
- CORREGIDO - en config contraste el límite inferior no se mostraba
- CORREGIDO - en gui about se retiró variable id, no se usa
- CORREGIDO - en chaser se quitó el label iniciar, no se usa
- CORREGIDO - en numérico calc se quitó la variable salida, no se usa
- CORREGIDO - en numérico calc se quitó la variable Num_Val_Temp_3, no se usa
- CORREGIDO - en chaser ya no guarda los valores de los cambios aplicados, al salir los regresa a su lugar
- CORREGIDO - en multiply cuando hace en cálculo se cambia apply por calc..
- CORREGIDO - en ubicar se agrega cancelar con center
- CORREGIDO - se cambió la url del about apuntando al Wiki

***

**v0.6 - Stable - Hardware v0.0 - v0.2**
- CORREGIDO - los valores limites superiores de config se escribían un carácter después
- CORREGIDO - hacer a partir de 155 el dimmer del contraste
- CORREGIDO - botón * de back light funciona errático - faltaba delay para evitar repetición
- CORREGIDO - quitar en config el dimmer 0-255, no aplica al contraste
- CORREGIDo - las io no usadas son salidas low
- CORREGIDO - no inicializa el contraste
- CORREGIDO - en matrix no se aplican los cambios en los bancos
- CORREGIDO - en matrix el valor final del banco se pasa de 512
- CORREGIDO - en config backlight el valor no se guardaba en eeprom
- CORREGIDO - en config backlight se recorrían todas las opciones de botones, se agregó mecanismo para sacar del bucle
- CORREGIDO - se bajó el delay de la lectura análoga para evitar pasos escalonados
- AGREGADO  - potenciómetro para valores DMX con tecla "D" solo en valores, para detenerlo presionar # o center
- AGREGADO  - análogo a unitary
- AGREGADO  - análogo a matrix
- AGREGADO  - análogo a config back light
- AGREGADO  - análogo a config contrast
- AGREGADO  - en la lectura análogo mecanismo para escribir el valor solo cuando cambia y no todo el tiempo

***

**v0.5 - Stable - Hardware v0.0 - v0.2**
- AGREGADO  - la función para cuando se da enter en un numero para cambiarlo, si de da enter de nuevo se quede el número que estaba

***

**v0.4 - Stable - Hardware v0.0 - v0.2**
- CORREGIDO - se retira del about el ID
- CORREGIDO - se cambia en config el menú exit por Ctrl
- AGREGADO  - void Back_Light_En() para encender o apagar el back light desde el teclado numérico
- AGREGADO  - void Back_Light_Init() para encender o apagar el back light desde la última configuración
- AGREGADO  - a Control Options el menú Config
- AGREGADO  - void GUI_Config() con las opciones de la configuración, el LCD y la salida al pwm
- AGREGADO  - control del back light a gui_navegar, siempre está activo
- AGREGADO  - se actualiza el about con el nombre del proyecto
- AGREGADO  - al config el about
- AGREGADO  - al about desde config espera a que se presione center para salir
- AGREGADO  - al config mas info sobre el backlight
- AGREGADO  - a control options Memory options
- AGREGADO  - en matrix la opción de poner el valor final de la matriz
- AGREGADO  - a la lectura numérica centro como enter

***

**v0.3 - Stable - Hardware v0.0 - v0.2**
- CORREGIDO - retirar de setup las variables de la versión y pasarlas directamente a su void
	    - no hay razón para que sean globales
- CORREGIDO - en gui about retirar el delay en el efecto binario
- CORREGIDO - eeprom save, load empty y clear retirar delay de efecto
	    - se retiró en todos los casos
- CORREGIDO - agregar al inicio del programa .ino un about
- CORREGIDO - en control chaser se quitó el espacio entre delay el número y x10=mS, parece que fuera una opción

***

**v0.2 - Stable - Hardware v0.0 - v0.2**
- CORREGIR  - retirar del setup las variables de la versión y pasarlas directamente a su void
- CORREGIR  - en GUI_About se retirar el delay en el efecto binario
- CORREGIR  - eeprom save, load empty y clear retirar el delay de efecto binario
- CORREGIR  - agregar al inicio del programa un about
- CORREGIR  - checar el tema del puerto de data flux, no se asigna
- CORREGIDO - se cambió gui_init por gui_about
- CORREGIDO - se cambia en unitary control, matrix por control y apunta a gui control options
- CORREGIDO - se cambia en matrix control, “ubi” por “con” y apunta a gui control options
- CORREGIDO - se quita la opción about es muy repetitiva
- AGREGADO  - control options about
- AGREGADO  - control options Chaser
- AGREGADO  - control options multiply
- AGREGADO  - actualización del texto "about"
- AGREGADO  - actualización del texto “memory initial”
- AGREGADO  - al GUI_Memory "empty" para borrar la ram
- AGREGADO  - el control multiply
- AGREGADO  - a about al inicio el efecto del binario corriendo

***

**v0.1 - Stable - Hardware v0.0 - v0.2**
- CORREGIDO - cambiar en gui unit a "Unitary"
- CORREGIDO - cambiar en GUI multi a "Matrix"
- CORREGIDO - hacer los barridos de la memoria más rápidos, se agrega efecto de carga y no baja la velocidad
- CORREGIDO - agregar al menú memory "Cancel"
- CORREGIDO - se agrega 100ms mas a la lectura de los cursores
- CORREGIDO - cuando se escribe un numero en la matriz o en unit, mayor o menor al límite la variable funciona pero el visual no
- CORREGIR  - en GUI_Multi no hay vista de posición
- AGREGADO  - líneas bajas cuando se está escribiendo un número, se quitaron los ceros
- AGREGADO  - se implementa para el caso de los valores "A" para 255 y "B" para 000
- AGREGADO  - se implementa para los valores la tecla "C" para ubicar la lámpara, parpadea y deja de hacerlo al volverla a presionar
- AGREGADO  - se implementa en la matriz el valor "C" que indica el canal donde está posicionado el cursor

***

**v0.0 - Beta - Hardware v0.0 - v0.2**
- Hello World !!

***