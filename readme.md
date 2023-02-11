# Desarrollo colaborativo

Esto es una guia teorico/practica para los alumnos de 'Git: Desarrollo colaborativo'__ que cursan los dias Lunes y Miercoles de 10 a 13 hs__ con el objetivo de reforzar conceptos y registrar los contenidos vistos en clase.

## Configuracion Inicial

Cuando descargamos una herramienta __GIT__ debemos inicializar un proyecto en una carpeta a eleccion, pero para poder confirmar los cambios realizados es necesario que tengamos establecidos un _nombre de usuario_ y un _correo electronico_.

Dicha informacion es necesaria para realizar los commits y ademas sirve para que los colaboradores del proyecto se contacten con nosotros. Para definir esta configuracion debemos utilizar los siguientes comandos.

* __git init__: inicializa el repositorio en la carpeta actual.
* __git config user.name 'name'__: define el nombre del usuario del colaborador para el proyecto.
* __git config user.email 'email'__ : define el correo de contacto.

## AREAS DE GIT

Cuando trabajamos con GIT, debemos tener en cuenta que el proceso para registrar los cambios se divide en etapas, las cuales corresponden a las diferentes areas que se detallan a continuacion:

1. ***WORKING DIRECTORTY:*** El area de trabajo corresponde a la carpeta donde creamos el repositorio y vamos a crear, editar y/o eliminar los archivos que forman parte del proyecto.
2. ***STAGING AREA:*** El area de control de cambios, tambien llamada index, se utiliza para realizar las capturas de codigo (SNAPSHOT) que luego deberan ser confirmadas si corresponde.
3. ***REPOSITORY:*** El almacen de cambios corresponde a una carpeta oculta que registra todo en archivos BLOB (Binary Large Object), y que podemos consultar utilizando el historial de confirmaciones.

## Gestion de Repositorios Remotos

Normalmente todos los cambios realizados se van a gestionar de manera local, pero una vez recopilado un conjunto de estos, necesitaremos publicar dichas modificaciones en un servidor git.Esto sucede principalmente para que podamos acceder a dicho repositorio desde cualquier ubicacion y tengamos una copia, a modo respaldo, de nuestro proyecto.

Algunos de los comando que se relacionan con con la gestion de repositorios remotos, ya sea para clonar el mismo o modificar:

___git clone 'url': __ clona un repositorio en el directorio actual.

__git remote add 'alias' 'url': __agrega una direccion de un repositorio remoto

__git remote rename 'old' 'new': __cambia el nombre de un repositorio remoto especificado
__git remote set-url 'remote' 'url': __modifica una direccion url del remoto seleccionado

## APUNTADORES GIT

*__HEAD:__ apuntador movil que indica donde nos encontramos dentro del historial de confirmaciones, tambien se utiliza como referencia para los comandos de git. Como por ejemplo: _git checkout__
*__BRANCH:__ apuntador dinamico que se asocia con el ultimo commit de la historia en la que nos encontramos, sirve para probar caracteristicas y realizar correcciones sin comprometer la rama principal.
*__TAG:__ apuntador estatico que se asigna a un commit en particular apra poder acceder al mismo sin necesidad de utilizar otra referencia, normamlmente se utiliza para el versionado del proyecto.
*__STACH:__ apuntador de la zona temporal de cambios (pila stash) que se utiliza de manera local, cuando necesitamos desplazarnos entre ramas y tenemos cambios pendientes, que no ameritan un commit.

## Contacto

Para mas informacion consultar la plataforma [Alumni](https://alumni.educacionIT), donde tambien pueden realizar los examenes.

Tambien pueden obtener mas detalles sobre 