# Instrucciones inicio del proyecto

### Paso 1: Instalar dependencias

Para poder utilizar el proyecto es necesario instalar las dependencias de este, tales como Leaflet para mapas y typeScript para desarrollo. Para esto hay que ejecutar la siguiente linea de comandos en consola:

```bash
npm install
```

### Paso 2: Iniciar Proyecto

Para poder iniciar el proyecto es necesario ejecuar el siguiente comando en consola:

```bash
ng serve
```

# Instrucciones de funcionamiento del frontend:

### Paso 1: Login

Al acceder al proyecto se mostrara el login por defecto (tambien al ingresar de path "localhost:4200/login").

En este componente es necesario ingresar un correo valido (no necesariamente real) que cumpla con el formato de correos (correo@example.com). Tambien se debe ingresar la contraseña (no tiene que ser real) para asi porfin acceder a la aplicacion web.

### Paso 2: Mapa

En este componente se cargara un mapa con leaflet el cual se cargara en base a la ubicacion actual del usaurio.

En este mapa apareceran algunos puntos (no reales) los cuales mostraran el estado del sensor.
- Funcionando: este estado muestra que el sensor esta funcionando sin anomalias.
- Detenido: este estado muestra que el sensor esta detenido.
- Fallido: este estado muestra que el sensor esta fallando dado a falta de comunicacion con los demas elementos.

### Paso 3: Registro

Esta funcionalidad permite al administrador crear un nuevo punto, esto se hara haciendo click sobre algun punto random del mapa.

Al hacer eso se cargara un componente con la latitud y la longitud ya cargados en el cual se le ingresara un nombre al punto.

Luego una vez ingresado el nombre se debe presionar siguiente para acceder al registro de conexion del sensor. Este punto muestra los inputs donde se ingresara la informacion para la conexion del sensor: nombre de este, SSID de la red a conectar y la contraseña de esta. Una vez añadidos todos los datos se presionara guardar y aparecera un nuevo punto en la ubicacion seleccionada (este punto se borrara al reiniciar el proyecto).