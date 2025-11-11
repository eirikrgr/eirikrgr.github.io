# Computer System Model
-

Para programar en C, siempre debes tener en cuenta: la CPU, memoria y como la CPU maneja los perifericos.
De nuevo, es muy importante tener en mente lo dicho anteriormente, C fue hecho para hacer la vida del programador 
mas facil, en 1970 siempre se programaban las CPU usando lenguaje ensamblador y era muy dificil, con "C" eso ya no es necesario.

**Nota** : Aqui un truco para entender mas sobre C; "En C cada declaracion es una operacion matematica, movimiento de dato o una operacion de memoria", tan simple como eso.


Load-Store model

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
Para lograr esto la CPU coloca la direccion de memoria deseada en el "Adress BUS" y lee o escribe los datos a traves del "Data BUS".
Cuando los datos son transferidos desde la memoria al registro es conocido como una operacion "load" o carga, mientras que mover datos del registro a la memoria es conocido como almacenamiento.
