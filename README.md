# :card_index: Introducción a SQL

## Objetivo
El objetivo de este taller es el de aprender a hacer consultas SQL en una base de datos relacional, en este caso utilizaremos PostgreSQL desde el gestor de datos pgAdmin. 

## Instrucciones
- Crea una base de datos llamada 'library'
- Crea una tabla llamada 'members'
- Crea 5 atributos:
	1. id -> de tipo númerico, que sea la clave primaria y se autoincremente
	2. dni_nie -> de tipo varchar, con límite de 9 caracteres
	3. name -> de tipo varchar, con límite de 150 caracteres
	4. lastname -> de tipo varchar, con límite de 150 caracteres
	5. birth_date -> de tipo date (YYYY-MM-DD)
- Crea 5 registros manualmente, para acceder a todos los registros haz click derecho sobre la tabla 'members' y selecciona View/Edit Data y haz click en 'All Rows'. Dentro de la pestaña Data Output haz click en el botón 'Add Row' y añade un registro, cuando completes todos los campos da click en 'Save Data Changes'. Recuerda que id no se debe rellenar ya que debe generar un id automáticamente.
- Los registros deben cumplir con los siguientes requisitos:
    1. Dos registros deben tener el apellido Alvarado y uno de ellos debe tener su fecha de nacimiento el 2020-05-08.
    2. Un registro debe tener el nombre María.
    3. Dos registros deben tener exactamente los mismos datos (excepto id).
    4. Las fechas de nacimiento serán variados y deben ir desde el 1 de enero del 1970 al 1 de enero del 2020.

## Ejercicio:
Cuando ya tengas creada la base de datos y la tabla, ingresa a tu base de datos y entra a Schemas/public/Tables/members y haz click derecho y escoge 'Query Tool', allí realizarás todas las siguientes consultas SQL:

1. Selecciona los registros cuyo apellido es Alvarado.
2. Selecciona todos los registros sólo con sus nombres y apellidos.
3. Inserta a la tabla 'members' un nuevo registro.
4. Inserta a la tabla 'members' 4 nuevos registros en una sola sentencia.
5. Selecciona todos los registros por orden alfabético ascendente por apellido.
6. Selecciona los registros que sean menores de edad.
7. Selecciona el id, nombre y apellido de los registros cuya fecha de nacimiento sea mayor al 1 de enero del 2018.
8. Selecciona todos los registros cuya fecha de nacimiento esté dentro del 1 de enero de 1990 al 1 de enero del 2020.
9. Actualiza al registro de nombre María a Valentina.
10. Elimina los registros que aparezcan con dni_nie repetido y deja solo 1 registro.
11. Añade una restricción en la columna dni_nie para que no permita valores repetidos.
12. Intenta crear un registro con un dni_nie que ya exista en tu base de datos (debería dar un error).

## Envío de la solución 
Copia cada sentencia en el archivo introToSql.sql y envía el taller.
