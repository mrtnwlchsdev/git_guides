# Git

- Sistema de control de versiones mediante el cual es posible seguir los cambios efectuados sobre un proyecto.
- Git permite realizar capturas de cada cambio realizado mediante commits.
- Cada commit realizado puede ser accedido nuevamente sin importar el avance del proyecto.

## Instalacion

    $ sudo apt-get install git

## Configuracion

Agregar un nombre de usuario e email al repositorio local de git

    $ git config --global user.name <user_name>
    $ git config --global user.email <user_email>

Obtener el nombre de usuario e email configurados

    $ git config --get user.name
    $ git config --get user.email

## Comandos basicos

Iniciar un repositorio de Git

    $ git init

Añadir recursos del proyecto al area de ensayo

    $ git add <file>

Verificar el estado del flujo de trabajo

    $ git status

Realizar un commit

    $ git commit -m <commit message>

Enviar los cambios alojados en el repositorio local de git, a un repositorio remoto (GitHub)

    $ git push

Enviar los cambios alojados en el repositorio remoto, al repositorio local de git

    $ git pull

Clonar un repositorio remoto en un sistema local

    $ git clone <origin>

## Comandos adicionales de git

Remover un recurso del area de ensayo

    $ git restore --staged <file_name>

Agregar archivos que contengan una extension especifica al area de ensayo

    $ git add *.html

Agregar todos los recursos contenidos en el directorio de trabajo al area de ensayo

    $ git add .

Deshacer los cambios realizados sobre un archivo

    $ git restore <file_name>

## Ignorar recursos

El archivo .gitignore contiene el nombre de los recursos que no seran añadidos al repositorio remoto.

    .gitignore\
        node_modules\
        test.html
        ...

## Trabajando con ramas

Por defecto la rama principal de un proyecto manejado mediante git se denomina como main.

Listar las ramas del proyecto

    $ git branch

Crear una nueva rama

    $ git branch <branch_name>

Pasar de una rama a otra

    $ git checkout <brnach_name>

