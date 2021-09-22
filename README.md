# Lab4uTest
Prueba técnica Frontend para Lab4U

## Tabla de contenidos
- [Introducción](#introducción)
- [Tecnologías usadas](#Tecnologías-Usadas)
- [Patrón-arquitectónico](#Patrón-arquitectónico)
- [Back-end](#Back-end)
- [Front-end](#Front-end)
- [Recursos](#Recursos)

## Introducción 
Esta es una prueba técnica para un puesto de practicante Front-end en Lab4U. Se pidió realizar un CRUD simple con una bd local, siguiento algún patrón arquitectónico, con tecnología libre y que fuera responsive. 

## Tecnologías Usadas
En este proyecto se usaron las siguientes tecnologías:
- C#
- ASP.NET 
- Entity Framework
- SQL Server
- Bootstrap

#### ¿Por qué estas tecnologías?
Las tecnologías utilizadas son de gran utilidad al momento de crear una aplicación web y permiten la implementación de modelos arquitectónicos con mayor fácilidad (mvc). Además son tecnologías que se buscan en la empresa y son las que necesitaré implementar en un futuro cercano para la construcción de mi portafolio de título. Así que son 2 pajaros de un tiro. 

## Patrón arquitectónico
El patrón arquitectónico utilizado en esta prueba fue Modelo Vista Controlador (**MVC**), utilizando las herramientas proveídas por Visual Studio para esto. 

## Back-end
En cuanto al back-end realizado para este CRUD, se utilizaron las tecnologías mencionadas anteriormente. 
La base de datos utilizada para almancenar los registros y que estos no se perdieran al cerrar la aplicación fue SQL Server 2019.
Para agilizar la creación del CRUD se utilizó el metodo Database First, haciendo que, una vez creada e implementada la base de datos, Entity Framework crea las clases, controladores y vistas bases automáticamente para trabajar con los datos desde la web de manera inmediata. 
Esto permite hacer la creación de un back-end sencillo en poco tiempo y útil en muchas otras ocaciones. Sin embargo carece de validaciones de campos, por los que estos los tuve que hacer de manera manual en el archivo `Usuario.cs`, donde se encuentran los getter y setters.

####validaciones
Los campos se encuentran validados de la siguiente manera:
- **Nombre** es un campo Requerido y debe contener al menos 2 caracteres, con un máximo de 50. 
Cada incumplimiento de lo mencionado cuenta con su respectivo mensaje de error que se mostrará debajo del input en las vistas al ser activado. 

- **Correo** es un campo Requerido  y debe contener al menos 2 caracteres, con un máximo de 50. Tiene que tener sintaxis de email, de lo contrario no será aceptado.
Cada incumplimiento de lo mencionado cuenta con su respectivo mensaje de error que se mostrará debajo del input en las vistas al ser activado. 



## Front-end
El Frontend de esta aplicación está hecho, como se mencionó al inicio, utilizando Bootstrap 4.6, HTML, CSS y Razor.

Para el desarrollo Front se aplicó la metodología **Mobile First**, para garantizar que se vea de manera correcta en cualquier dispositivo desde smartphones a Monitores normales. Por esto las vistas se desarrollaron mayoritariamente con el navegador en modo Mobile S (320px), que corresponde a la medida más pequeña para teléfonos.

Bootstrap fue utilizado principalmente para realizar la parte responsive dejando el diseño de elementos en su mayoría al CSS puro y duro. 

Se utilizó Font-Awesome para la implementación de Iconos a lo largo de las vistas.

Los campos de formularios también se encuentran validados mediante las etiquetas html.

#### Accesibilidad
El tamaño de la fuente fue cambiado en el css, para permitir el reemplazo de PX por **REM** en el font-size. Esto para permitir que personas con problemas de visión puedan ver más claramente las palabras, ya que rem es una medida relativa, no como px que es una medida absoluta, por lo que rem se adapta al tamaño de la letra que tenga por defecto en el navegador.

## Recursos
Links a los recursos utilizados para este proyecto:

- [SQL Server](https://www.microsoft.com/es-es/sql-server/sql-server-downloads "SQL Server")
- [Font-Awesome](https://fontawesome.com/v4.7/ "Font-Awesome")
- [Bootstrap](https://getbootstrap.com/docs/4.6/getting-started/introduction/ "Bootstrap")
- [Visual Studio](https://visualstudio.microsoft.com/es/vs/ "Visual Studio")






