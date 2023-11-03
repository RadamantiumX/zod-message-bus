# ZOD MESSAGE BUS

Utilizando la gestion de las paqueteria con PNPM, en esta libreria se desarrollará un sistema de solicitudes con el uso de ZOD, otra libreria destina a la validacion de los datos que estamos peticionando.

Dentro de las principales librerias q vamos a utilizar esta TSUP, la cual se encargara del empaquetamiento a BUILD de este proyecto.

## SINTAXIS IMPORTANTE

Al modificar el script (en el package.json), dar especial atencion a los espacios que se dejan en el STRING, por ejemplo, la forma correcta de modificar la BUILD, es de esta manera:

```
 "build": "tsup src/index.ts --format cjs,esm --dts"
``` 

Y **NO** esta:

```
  "build": "tsup src/index.ts --format cjs, esm --dts" 
```  

Como se pude observar, espacio en la definicion de las extenciones puede perjudicar el empaquetado.
