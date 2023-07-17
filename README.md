# Proyecto BlockBuster

Este repositorio es una aplicación web desarrollada con Ruby on Rails que simula un sistema de registros de arriendo de películas para un BlockBuster ficticio.
![img](https://github.com/toffycaluga/Blockbuster-inforcap/blob/main/app/assets/images/Blockbuster.png)

## Requisitos

- Ruby 3.1.1
- Rails 7.0.4
- PostgreSQL (base de datos)
- Faker 2.23 (para generar datos ficticios)

## Instalación

1.  Clona el repositorio desde GitHub.
    git clone https://github.com/toffycaluga/Blockbuster-inforcap.git

2.  Ingresa a la carpeta del repositorio

        cd Blockbuster-inforcap

3.  Instala las gemas necesarias.
    bundle install

4.  Crea la base de datos y migra las tablas .
    rails db:crete
    rails db:migrate

5.  Carga datos ficticios.
    rails db:seed

## Uso

Una vez que hayas realizado la instalación , puedes ejecutar la aplicación localmente con el siguiente comando:

        rails s

La aplicación estará disponible en `http://localhost:3000/`.

## Funcionalidades

- **Registro de películas:** Los usuarios pueden registrar películas con su título y cliente que la arrendo.

- **Registro de clientes:** Los usuarios pueden registrar nuevos clientes con su nombre y edad.
- **Arriendo de películas:** Los usuarios pueden asignar películas a clientes, de modo que un cliente solo pueda tener una película arrendada a la vez.

- **Visualización de películas arrendadas:** En la página de clientes, se muestra si el cliente tiene una película arrendada y, en caso afirmativo, cuál es la película.

## Paso a paso para subir a heroku

1. Crea una cuenta o inicia sesión en Heroku en https://www.heroku.com/.

2. Una vez que hayas iniciado sesión, en el Dashboard de Heroku, haz clic en el botón "New" (Nuevo) y selecciona "Create new app" (Crear nueva app).

3. En la página "Create new app", ingresa un nombre para tu aplicación y selecciona la región más adecuada.

4. Luego, en la pestaña "Deploy" (Desplegar) de la página de tu aplicación, en la sección "Deployment method" (Método de despliegue), elige la opción "GitHub" (también puedes elegir Git si has subido el código a GitHub previamente).

5. Conecta tu cuenta de GitHub a Heroku y busca el repositorio del proyecto en la lista.

6. Después de conectar el repositorio, puedes elegir entre desplegar la rama principal automáticamente o desplegar manualmente eligiendo la rama.

7. Una vez que hayas configurado el despliegue, ve a la pestaña "Settings" (Configuraciones) y haz clic en "Reveal Config Vars" (Mostrar variables de configuración).

8. Agrega todas las variables de entorno necesarias para tu aplicación. Asegúrate de configurar la clave secreta de Rails y cualquier otra variable que necesites.

9. Ahora, en la pestaña "Resources" (Recursos), asegúrate de que esté habilitado el servicio de base de datos PostgreSQL para tu aplicación. Si no lo está, agrégalo seleccionando "Heroku Postgres" en la sección "Add-ons".

10. Una vez que hayas configurado todo, haz clic en el botón "Deploy Branch" (Desplegar rama) en la pestaña "Deploy" para iniciar el despliegue de tu aplicación.

11. Heroku comenzará a desplegar la aplicación y podrás ver el progreso en los registros (logs). Si todo va bien, la aplicación debería estar disponible en la URL de Heroku.

⌨️ con ❤️ por [Toffy Caluga](https://github.com/toffycaluga)
