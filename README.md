# carro-seguidor-de-linea
CREACION DE CIRCUITOS ELECTRONICOS CON MICROCONTROLADORES
PLAN DE TRABAJO
ING. JUAN JOSE GUEVARA
ALUMNOS: 
Lara González, Cristopher Alejandro			346318
Ventura Sánchez, Fátima Edelmira                           341018
Facundo Rivas, Jocelyn Estefany 			         165218  
			
GRUPO: HAR21-B
 
DESCRIPCION DEL PROYECTO
Nuestro proyecto consiste en un carro seguidor de línea, micro controlado con un PIC 18f4550, el cual tendrá las medidas de 6cm de altura incluyendo el alto de las llantas, 14 cm de ancho y 18cm de largo, el diseño será de forma rectangular, la base del carro será de acrílico,  llevara cuatro sensores CNY70 distribuidos los cuatro adelante, de  los cuales cada uno de ellos posee dos leds, un emisor y un receptor, los cuales funcionan de la siguiente manera: el led emisor emite luz y el led receptor recibe, si el led receptor recibe un 0 lógico entonces le manda un 1 lógico a la salida indicando que este se encuentra sobre un área de color negro, en dicho caso el carro va a caminar o avanzar hacia adelante y si el led receptor recibe un 1 lógico entonces manda un 0 lógico a la salida indicando que se encuentra sobre área blanca, lo cual significa que no se va a mover, las señales enviadas por los sensores llegan como entradas digitales a nuestro Pic 18f4550, esta información es procesada y evaluada por el programa cargado al Pic 18f4550, dicho programa contiene estructuras if que evalúan todas señales  enviadas por los sensores, cuando las señales de los sensores delanteros sea 1 entonces el carro va a caminar hacia adelante, y en el momento en que todos los sensores envíen 0 lógico no se va a mover por ninguna circunstancia, y dependiendo de los resultados se envían los datos a las salidas digitales  asignadas que irán conectadas a los drivers,  dichos datos al ser procesados en el PIC 18f4550 son mandados a los drivers L293D, que nos permitirán controlar a los motores DC que se utilizaran  para las cuatro llantas que llevara nuestro carro seguidor de línea,  al recibir los datos el L293D directamente envía los datos a los cuatro motores para que realicen la acción debida para cada caso, ya sea caminar hacia adelante, girar hacia la derecha, girar hacia la izquierda o detenerse al detectar zonas blancas.
METAS PARA EL PROYECTO
1)	Lograr tener el mayor dominio sobre los temas impartidos en clase, aplicándolos en la elaboración de un carro seguidor de línea.
2)	Desempeñar el proyecto acorde el tiempo estipulado y asegurarnos que vaya lo mejor posible tanto en el hardware como en el software. 
3)	Demostrar los conocimientos de cada uno adquiridos a lo largo de todo el modulo en la defensa del proyectoISEÑO DEL CHASIS
CRONOGRAMA DE ACTIVIDADES
CRONOGRAMA
SEMANAS	DESCRIPCION
Semana 1	•	Elaboración del plan de trabajo
•	Crear el diseño del chasis.
•	Crear el diseño del P.B.C. de:
-	Sensores
-	Drivers
-	Otros
•	Subir a Github.
Semana 2	•	Elaboración de la placa para los drivers.
•	Elaboración de las placas de los sensores. 
•	Ajustes y ensamblado al carro.
•	Subir avances en Github
Semana 3	•	Elaboración del código para el carro seguidor de línea.
•	Prueba del recorrido al carro en la pista.
•	Ajustes finales al carro.
•	Elaboración del Paper IEEE sobre el proyecto del carro.
•	Subir los avances a Github
Semana 4	•	Defensa del proyecto en la clase de teoría.
•	Defensa y demostración del carro en el laboratorio de práctica.
•	Subir el avance final a Github.

PRESUPUESTO ESTIMADO
Cantidad	Componente	Precio
2	Integrado L293D	$10.62
2	Base para integrado de 16 pines	$2.00
4	Sensor CNY70	$10.80
4	Llantas con Motores DC	$12.16	
1	Placa de cobre	$9.00
TOTAL	$44.48

