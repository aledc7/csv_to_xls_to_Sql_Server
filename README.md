![xls to sql server](https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/import-excel-to-sql.png "github.com/aledc7/xls_to_sqlServer")



[![aledc.com](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/aledc.com.svg)](https://aledc.com)
[![ingenea.com.ar](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/ingenea.svg)](http://ingenea.com.ar)
[![License](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/mit-license.svg)](https://aledc.com)
[![GitHub release](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/release.svg)](https://aledc.com)
[![Dependencies](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/dependencias-none.svg)](https://aledc.com)




## How to Convert any CSV or XLS file into SQL Server Table

## Como convertir cualquier archivo CSV o XLS en una tabla de SQL Server


Requirements

- [x] Sql Server Management Studio
- [x] Excel 2010 or +


1.  
The content of a .csv file separated by commas is displayed.
First we will convert this file into xls

Se muestra el contenido de un archivo .scv separado por comas.  
Primero convertiremos este archivo en xls

<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/excel1.png" width="500"
</p>


Se observa en la imgen de arriba, que todos los datos del archivo csv se encuentran en la misma columna, lo primero que haremos será separar cada campo en una columna, estos son los pasos:




## Convirtiendo un archivo CSV a XLS


1.  Abrir un documento de excel en Blanco y Luego seleccionar el menú de __importar__

<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/excel2.png" width="500"
</p>
  
  
  
2.   Seleccionar el tipo __CSV__


<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/excel3.png" width="500"
</p>
  
  
  
3.  Definir a partir de que fila se comienza la importación, en mi caso desde ela fila 1.

Luego elijo __Unicode (UTF8)__  y el radio buton en __Delimited__

<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/excel4.png" width="500"
</p>
  
4.  Aquí debo indicar que caracter separa los campos en el archivo csv, en mi caso es una coma. 
Aqui ya se debería notar la divisio de las columnas, en caso contrario, seguir cambiando la configuración, hasta lograr la división, tal como se muestra en la imagen de abajo :point_down:
  
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/excel5.png" width="500"
</p>


5.  En este paso es posible indicar el nombre de cada columna, o biene elgir que una fila sea la que determine el nombre de las columnas.
 En mi caso, la primer fila del archivo contenia el nombre de la columna, por lo que no es necesario escribir nada.

  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/excel6.png" width="500"
</p>


6.  Aqui pregunta en que hoja del archivo excel se copiaran los datos.
 Esta operacion puede tomar bastante tiempo, dependiendo del tamaño del archivo.

  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/excel7.png" width="500"
</p>


7.  Finalmente podemos observar el archivo de excel con sus datos separados por columnas.

  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/excel8.png" width="500"
</p>


8.  Solo resta guardarlo con extensión  __xls 97-2004__ ya que este es el formato que usaremos en los pasos siguientes

  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/excel9.png" width="500"
</p>

## Parte SQL


1.

Una vez tenemos creado el archivo xls separado por columnas, procedemos a abrir el __SQL Management Studio__  

Luego de estár logueado y conectado, damos click secundario sobre la base que datos a la cual queremos insertarle la nueva tabla, y elegimos __Tasks__ luego __Import Data__ 

Database :arrow_right: __Tasks__ :arrow_right: __Import Data__

<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/slq1.png" width="500"
</p>


2.  Se abrirá el Wizzard , le damos siguiente  :point_down:

<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql2.png" width="500"
</p>
  






3. Luego en __Data Source__ elegimos __Microsoft Excel__


 <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql3.png" width="500"
</p>


4. Exploramos y seleccionamos el archivo xls que será convertido en tabla 
  



5. Luego debemos asegurarnos de tildar  - [x] First row has column names
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql4.png" width="500"
</p>

6. Luego en __Choose a Destination__ se debe seleccionar __Microsoft OLE DB Driver for SQL Server__ como se muestra en la foto :point_down:
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql5.png" width="500"
</p>


7. Luego en esta pantalla se debe indicar el nombre del servidor, la base de datos de destino, y las credenciales de __User__ y __Password__
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql6.png" width="500"
</p>


8.  Luego se debe seleccionar __Copy data from one or more tables or views__  
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql7.png" width="500"
</p>


9. En este cuedro muestra el __origen__ y __destino__ de la migración.
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql8.png" width="500"
</p>
  
10. Por ultimo verificar que se encuentre checkeado el icono de __run inmediately__   
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql9.png" width="500"
</p>


11. Confirmar haciendo click en __finish__
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql10.png" width="500"
</p>
  
12. Si todo fue exitoso debería verse la siguiente imágen :point_down:  
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql11.png" width="500"
</p>


  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql12.png" width="500"
</p>
  
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql13.png" width="500"
</p>
  
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql14.png" width="500"
</p>
