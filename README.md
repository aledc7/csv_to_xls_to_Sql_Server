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
  
4.  Aquo debo indicar que caracter separa los campos en el archivo csv, en mi caso es una coma. 
Aqui ya se debería notar la divisio de las columnas, en caso contrario, seguir cambiando la configuración, hasta lograr la división, tal como se muestra en la imagen de abajo :point_down:
  
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/excel5.png" width="500"
</p>


5.

  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/excel6.png" width="500"
</p>


6.

  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/excel7.png" width="500"
</p>


7.

  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/excel8.png" width="500"
</p>


8.

  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/excel9.png" width="500"
</p>

## Parte SQL


<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/slq1.png" width="500"
</p>
  
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql2.png" width="500"
</p>                       
  
  
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql3.png" width="500"
</p>
  
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql4.png" width="500"
</p>
  
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql5.png" width="500"
</p>
  
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql6.png" width="500"
</p>
  
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql7.png" width="500"
</p>
  
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql8.png" width="500"
</p>
  
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql9.png" width="500"
</p>
  
  <p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/xls_to_sqlServer/master/resources/sql10.png" width="500"
</p>
  
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
