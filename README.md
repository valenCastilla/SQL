# SQL

Este repositorio es una guía con todos los trabajos prácticos solicitados en la materia de "SQL" dentro de la "Licenciatura en Ciencia de Datos".


------------------     TP 1     ------------------      

TP grupal (max3 x grupo):  Investigar sobre: SQL, SGBD, DDL, DML.


------------------     TP 2     ------------------

2)	TP grupal (max 5 x grupo):  

a)	 Defina los siguientes términos : DER, Entidad, Interrelación (relationship), Conjunto de interrelaciones, Grado de una interrelación, Atributos , Identificador único, Evento. 
 
  b)	SQL

  	 i.	Para que sirve el SQL  ?

  	 ii.	En que etapa del ciclo de vida de un proyecto informático se utiliza el modelado con el SQL ?

  	iii.	Qué relación debe existir entre un SQL y un DBM ?


------------------     TP 3     ------------------

3)	Video Club: Discutir acerca de los procesos y necesidades de datos de un sistema para un VIDEOCLUB: Alquiler, Reserva, Compra de Nuevas Peliculas, Devolución.
  1.	Seleccionar una herramienta para su documentación
  2.	Realizar el Diagrama Entidad Relación
  3.	Realizar el DDD


------------------     TP 4     ------------------

4)	Una agencia de viajes necesita adoptar un sistema que le permita disponer de la siguiente información :


  	a.	Por cada cliente desea saber el código de cliente, nombre, dirección, teléfono, ocupación    y datos del grupo familiar.

  	 b.	Por cada Tours organizado por la empresa debe saber código de Tours, fecha y hora de salida fecha y hora de llegada, canti¬dad de plazas, nombre de la guía de turismo y las escalas que va realizando el Tours con hora y día de llegada y tiempo de esta¬día.

  	c.	La Empresa tiene contratada gente especializada en cada escala que acompaña a los Tours que pasa en su zona.

  	d.	El importe de cada Tours se puede pagar de varias formas.  Se debe registrar las cuotas pagas de cada cliente que corresponda a esta modalidad de pago.

  	 e.	El sueldo de los guías de turismo se deduce de un sueldo básico de acuerdo al cargo, más un importe por antigüedad, más un adicional por cada Tours que atendió.

	
 Se pide :
	  Hacer el DER indicando para cada entidad su identifica¬dor único y atributos.



------------------     TP 5     ------------------

5)	Sistema de administración de aeropuertos

Se quiere modelizar un sistema para la administración de aeropuertos. Se sabe que un aeropuerto trabaja con distintas líneas aéreas (Ej.: Aerolíneas Argentinas, Iberia, Air France, etc.) y una misma línea aérea trabaja en uno o varios aeropuertos.

A su vez un aeropuerto tiene varios mostradores de check-in que son adjudicados a las distintas líneas aéreas (Ej.: Iberia tiene asignados los mostradores 1, 2 y 3 del aeroparque de Ezeiza). De cada mostrador se conoce el número que lo identifica, el lugar donde está ubicado y el tipo de mostrador que puede ser “turista”, “primera clase” o “business”.

Los aeropuertos también tienen pistas que pueden ser pistas de despegue o pistas de aterrizaje y que son utilizadas por los aviones pertenecientes a las líneas aéreas en una fecha y hora dadas. Los aviones se clasifican según la cantidad de asientos en “avionetas” (de 2 a 4 asientos), “aviones medianos” (de 5 a 100 asientos) y “aviones boeing” (más de 100 asientos).

Cada avión tiene programados distintos vuelos, de los cuales se conoce: tipo de vuelo (charter o de línea), ciudad de origen (ciudad de donde sale el vuelo), ciudad de destino (ciudad a donde llega el vuelo), fecha de salida, hora de salida y una duración estimada.

De cada vuelo se pueden realizar reservas. Para esto la persona que realiza la reserva debe informar su nombre y el nro. de vuelo que desea, y la línea aérea le asigna un código de reserva alfanumérico y una fecha de vencimiento de la reserva. 

Cuando la fecha del sistema sea mayor que la fecha de vencimiento, las reservas que aún no hayan sido canceladas vencen, mientras tanto permanecen activas. 

La persona que compra un pasaje correspondiente a un vuelo dado debe informar su nombre, el tipo y el nro. de documento y es considerada para el sistema como “pasajero”.

Aclaraciones:
- Un mostrador es adjudicado a una sóla línea aérea o a ninguna (puede estar sin asignar por algún período de tiempo).
- Un avión pertenece a una única línea aérea que a su vez tiene varios aviones.
- Una reserva es adjudicada a una única persona, que puede realizar varias reservas (siempre de distinto vuelo).
- Una pista corresponde a un aeropuerto en particular, y es utilizada por varios aviones, que a su vez utilizan varias pistas.

Instrucciones:
    1.	Leer el enunciado, subrayar los sustantivos
    2.	Identificar las relaciones entre subrayando los verbos
    3.	Seleccionar una herramienta CASE
    4.	Elaborar el DER


------------------     TP 6     ------------------

6)	Pase los siguientes esquemas de relaciones a DER que lo represente fielmente.

AEROPUERTO (nombre-aeropuerto, ciudad)

VUELO (nro_vuelo, día_hora_salida, aeropuerto_origen, aeropuerto_destino)

ESCALA (nro_vuelo, aerop_desde, aerop_hasta)


------------------     TP 7     ------------------

7)	Dados los siguientes esquemas realice el DER correspondiente:


A(a1 a2, a3, a4)

B(b1 , b2,  b3,  b4)

C(c1 ,c2, c3, a1, a2)

D(c1 d1, d2, d3, d4)

E(b1 c1 , e1)


------------------     TP 8     ------------------

8)	Seleccionar un RDBMS.

a.	Verificar que esté correctamente instalado, o instalarlo.
  
  b.	Escribir el código SQL que define las tablas del ejercicio práctico Nro. 3 al 5



------------------     TP 9     ------------------

9)	Escribir el código SQL que define las tablas del ejercicio práctico Nro. 5

  	a.	Escribir el código SQL que define las tablas normalizadas (DDL)

  	 b.	Seleccionar los Vuelos de la Linea Aerolineas Argentina que despegaron en el mes de Marzo de 2011.

  	c.	Seleccionar las personas que volaron en Bussiness a Madrid.

  	d.	Informar la reserva de “Hugo López” para el mes que viene.

  	e.	Insertar en una tabla un registro completo. Imprimir una consulta previa (QUERY) en donde se evidencie que el registro no existía y luego la misma con ese registro. Incluir el código.

  	f.	Eliminar de una tabla un registro completo. Imprimir una consulta previa (QUERY) en donde se muestre el registro y luego la misma sin ese registro. Incluir el código.

  	g.	Hacer una consulta que indexe en otro orgen que no sea la clave primaria.

  	 h.	Hacer una consulta que agrupe datos e indique cantidad de registros que cumplen la agrupación de datos, ordenando en orden descendente.

  	i.	Utilizar InnerJoin

  	j.	Utilizar OuterJoin

  	k.	Aplicar los conocimientos adquiridos de optimización de consultas


------------------     TP 10     ------------------

10)	Escribir el código SQL que define las tablas del ejercicio práctico Nro. 4

   	a.	Escribir el código SQL que define las tablas normalizadas (DDL)

   	 b.	Seleccionar los Guias que mas trabajaron.

   	c.	Seleccionar las personas que mas viajaron.

   	d.	Informar el viaje de “Hugo López” para el mes que viene.

   	e.	Insertar en una tabla un registro completo. Imprimir una consulta previa (QUERY) en donde se evidencie que el registro no existía y luego la misma con ese registro. Incluir el código.

   	f.	Eliminar de una tabla un registro completo. Imprimir una consulta previa (QUERY) en donde se muestre el registro y luego la misma sin ese registro. Incluir el código.

   	g.	Hacer una consulta que indexe en otro orgen que no sea la clave primaria.

   	h.	Hacer una consulta que agrupe datos e indique cantidad de registros que cumplen la agrupación de datos, ordenando en orden descendente.

   	i.	Utilizar InnerJoin

   	j.	Utilizar OuterJoin

   	k.	Aplicar los conocimientos adquiridos de optimización de consultas



------------------     TP 11     ------------------

11)	Escribir para el TP 4, un SP, una Function y 2 Trigger. Implementarlo y mostrar su funcionamiento.


------------------     TP 12     ------------------

12)	Escribir para el TP 5, un SP, una Function y 2 Trigger. Implementarlo y mostrar su funcionamiento.










    
