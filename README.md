# PRUEBA TECNICA KONECTA

Para la ejecucion del proyecto se necesita importar la base de datos adjunta (cafeteriaSQL).

Añadir el Jar jcalendar-1.4.jar utilizado para deplegar calendario y el mysql-connector-java-5.1.13-bin

## CONSULTAS SQL
-Realizar una consulta que permita conocer cuál es el producto que más stock tiene.

  SELECT * FROM productos WHERE stock IN (SELECT MAX(STOCK) FROM productos)

-Realizar una consulta que permita conocer cuál es el producto más vendido.

  SELECT * FROM ventas WHERE id_producto IN (SELECT MAX(id_producto) FROM ventas
  
### Notas

Traté de realizar al 100% la prueba pero por temas de tiempo no logré realizarla en su totalidad.
