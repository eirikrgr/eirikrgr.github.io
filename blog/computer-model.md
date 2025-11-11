# Computer System Model
-

Para programar en C, siempre debes tener en cuenta: la CPU, memoria y como la CPU maneja los perifericos.
De nuevo, es muy importante tener en mente lo dicho anteriormente, C fue hecho para hacer la vida del programador 
mas facil, en 1970 siempre se programaban las CPU usando lenguaje ensamblador y era muy dificil, con "C" eso ya no es necesario.

**Nota** : Aqui un truco para entender mas sobre C; "En C cada declaracion es una operacion matematica, movimiento de dato o una operacion de memoria", tan simple como eso.


## Load-Store model

Un simple modelo de computacion puede ser el de una CPU conectada algun sistema de almacenamiento\
con la caracteristica de enviar instrucciones y datos.

<br>
<img src='./images/simple-cpu-model.png'>


Dentro de la CPU (Central processing unit), vemos algo llamado Register file (R0,R1,R2, etc), 
esto funciona como un almacenamiento temporal donde la CPU puede realizar algunas operaciones
- sumar.
- restar.
- dividir.
- comparar.
- Entre muchas otras operaciones.

La CPU puede manipular los datos almacenados dentro del registro. Sin embargo, los datos pueden ser transferidos entre el registro y la memoria usando el BUS. 
Para lograr esto la CPU presenta la direccion de memoria deseada "Adress BUS"
y escribe o lee los datos a traves del "Data BUS". 
Cuando los datos son transferidos desde la memoria al registro es conocido como una operacion "load" o carga,
mientras que mover datos del registro a la memoria es conocido como "store" o guardar.

Hay algo muy interesante que podemos notar en la imagen y es que **el periferico (LED) es tratado como una memoria!**,
esto significa que podemos leer y escribir en la direccion correspondiente al periferico, 
lo cual resultaria en una interaccion con el mundo real y todo desde nuestra CPU;
Por ejemplo el LED podria iluminar cuando algo se escriba en su direccion de memoria.


## Storage, Data and Instructions

Memoria. Es un componente fundamental de un sistema de computacion y opera en el nivel de los bits.
Cada bit esta compuesto de elementos electricos que representan una presencia o ausencia de carga electrica.
Esta distincion traduce el sistema binario donde la presencia de carga corresponde a "1" o al estado de "encendido" y por el contrario la ausencia de carga se traduce como "0" o estado de "apagado". 
Con 8 bits tenemos un byte y con 4 bytes combinados podemos formar una palabra.

La CPU interactua con la memoria por partes y no accediendo a bits individuales.
Esta puede leer o escribir datos en unidades de 1,2 o 4 bytes dependiendo de la arquitectura. El acceso directo a los bits no es posible, sin embargo el contenido almacenado en la memoria es esencialmente
una coleccion de bits. Como la CPU trata e interpreta aquellos bits es lo que distingue entre dos conceptos cruciales: "Data" and "Instruction".




