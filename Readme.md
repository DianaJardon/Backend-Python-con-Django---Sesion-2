## Backend(Python) con Django - Sesion 2

<span style="color: cyan">Instalar libreria</span>

1. Instalar a traves del pipenv
   
       $ pipenv install psycopg2-binary==2.8.6

<span style="color: cyan">Configurar base de datos</span>

Settings

![aliados](img/1.PNG)

Crear el proyecto Books

    $  python manage.py startapp books

Crear los modelos 

![aliados](img/2.PNG)

Crear una migración

    $ python manage.py makemigrations

![aliados](img/3.PNG)

Visualización de los cambios

    $ python manage.py sqlmigrate books 0002

![aliados](img/4.PNG)

Generar transacción a la base de datos con el siguiente comando:

    $ python manage.py migrate

Generar realciones

![aliados](img/5.PNG)

Realizar nuevamente el comando:

    $ python manage.py makemigrations

Como es una relación (un campo nuevo en una tabla que ya existe), preguntara lo siguiente: 

Seleccionamos la opción 2

![aliados](img/6.PNG)

Agregamos esta parte:

![aliados](img/7.PNG)

realizamos nuevamente la migración, ya no genera la pregunta anterior.

![aliados](img/8.PNG)

Hacer el migrate nuevamente

![aliados](img/9.PNG)

Verificamos las base de datos y las tablas que creamos:

![aliados](img/10.PNG)

Realizar una **Vista** (tipo GET)

Modificar el archivo urls y views

    $ python manage.py runserver 0.0.0.0:8000

![aliados](img/11.PNG)

Realizar una **Vista** (tipo POST)

Modificar el archivo urls y views

Visualizar la vista con el siguiente comando y al momento de entrar al servidor colocar  /authors/create/ ()

![aliados](img/12.PNG)

Agregamos contenido y manda el mensaje de creado

![aliados](img/13.PNG)

verificamos en la parte de authors

![aliados](img/14.PNG)

![aliados](img/15.PNG)

Visualisación los registros de forma grafica en PostgreSQL

![aliados](img/16.PNG)