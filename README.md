README
                                                   
                                                      


- TAREAS WEB APP

Esta es una aplicación web simple para gestionar tareas utilizando Flask y una base de datos Access. Permite a los usuarios ver una lista de tareas, agregar nuevas tareas, marcar tareas como completadas y eliminar tareas.

- REQUISITOS

Antes de ejecutar esta aplicación, asegúrate de tener instalados los siguientes componentes:

Python 3.x
Flask
pyodbc
Microsoft Access Driver (para acceder a la base de datos Access)


- CONFIGURACION

1. Clona o descarga este repositorio en tu computadora.

2. Asegúrate de tener una base de datos Access (.accdb) con una tabla llamada "Tareas" que tenga los siguientes campos:

    - Id (número de identificación único)
    - descripcion (texto, descripción de la tarea)
    - estado (entero, 0 para tareas no completadas y 1 para tareas completadas)

3. Abre el archivo app.py y modifica la línea de conexión a la base de datos (conn) para que apunte a tu archivo .accdb:

    conn = pyodbc.connect(r'DRIVER={Microsoft Access Driver (*.mdb, *.accdb)};'
                        r'DBQ=/ruta/a/tu/ArchivoDB.accdb;')

4. Instala las dependencias de Python ejecutando el siguiente comando en la terminal:
	pip install flask pyodbc

- USO

1. Ejecuta la aplicación con el siguiente comando:
    python app.py

1. Abre tu navegador y accede a http://localhost:5000/ para ver la lista de tareas disponibles.

2. Puedes agregar nuevas tareas completando el formulario en la página principal.

3. Para marcar una tarea como completada, haz clic en el enlace correspondiente junto a la tarea.

4. Para eliminar una tarea, haz clic en el enlace de eliminación junto a la tarea.

- CONTRIBUCIONES

Si deseas contribuir a este proyecto, siéntete libre de crear un Pull Request o informar sobre problemas.

¡Disfruta de la gestión de tus tareas con esta simple aplicación web!
