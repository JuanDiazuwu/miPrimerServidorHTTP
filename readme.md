# Práctica | Mi Primer Servidor HTTP

Desarrollo Basado en Plataformas

## Unidad II

Conceptos Básicos de las Plataformas Web

## Instrucciones

La practica consiste en crear un servidor en node.js en las siguientes etapas:

1.- Hola mundo básico.

2.- Servidor simple de hola mundo en node.js usando HTTP.

3.- Servidor síncrono que lea y envíe un archivo.

4.- Servidor asíncrono que lea y envíe un archivo.

5.- Servidor asíncrono que lea y envíe un archivo según su extensión.

6.- Agregar archivo README.md.

Suba la practica realizada en clase a github ó gitlab (con repositorio público) a la plataforma.

## Lenguaje de Programación 

JavaScript (Node.js v18.13.0.)

## Autor

**Juan Antonio Díaz Fernández**

	Usuario: JuanDiazuwu

	Matricula: 348637

* Personal [Github](https://github.com/Fuan200/) 
* Escuela [Github](https://github.com/JuanDiazuwu)

## Funcionamiento

El archivo `app.js` hace la implementación de un servidor web HTTP hecho en `Node.js` utilizando el modulo `http` y el `fs`.

La función que se encuentra en este archivo es `createServer`, crea un servidor HTTP, recibé como parámetros `request` y `response`, representan la solicitud y la respuesta de HTTP.

Se declará una constante `file` utilizada para obtener la ruta del archivo solicitado. Si la solicitud es la raíz del sitio web `/` se regresa el archivo llamado `index.html`, que tiene su ubicación dentro de la carpeta `./WWW`, si no se devuelve el archivo solicitado de dentro de `./WWW`.

La función `readFile` de `fs`, recibe como parámetro, el archivo y una función flecha que tiene `err` y `data`.
Se lee el archivo y la respuesta dependerá de la extensión del archivo solicitado. Si el archivo no es encontrado la respuesta es `404 Not found`.
Si el archivo es encontrado la respuesta es `200` y se muestra el archivo.

El servidor se aloja en el puerto `4444`.

## Instrucciones de Uso

* 1 .- Clona el repositorio.

* 2 .- Abre una terminal en la raíz del repositorio clonado.

* 3 .- Asegurese de tener instalado node.js

* 4 .- Ejecutar el siguiente comando en la terminal:

```
node app.js
```

Esto hará que el servidor se inicialize.

* 5 .- Abrir tu navegador de confianza.

* 6 .- EN la barra de busquedas escribir:

```
localhost:4444
```

Esto mostrará la pagina principal del sitio web.

* 7.- Si se quiere acceder a la pagina `about` en la barra de busquedas poner:

```
localhost:4444/about.html
```

* 7.- Si se quiere acceder a la pagina `login` en la barra de busquedas poner:

```
localhost:4444/registro.html
```

* 8 .- Para apagar el servidor, dirijase a la terminal de antes y haga `Ctrl + C`,

Siéntase libre de clonar este repositorio y probar su funcionamiento. ¡Espero que le sea útil!