# README - Métodos de Fecha en JavaScript

Este documento describe una serie de métodos proporcionados por el objeto `Date` en JavaScript para manipular fechas. A continuación se presenta una lista de métodos junto con ejemplos de uso:

## Métodos de Obtención de Información

### getDate()
Devuelve el día del mes (de 1 a 31).

```javascript
const fecha = new Date();
const diaDelMes = fecha.getDate();
console.log(diaDelMes); // Ejemplo de salida: 13
```

### getDay()
Devuelve el día de la semana (de 0 a 6).

```javascript
const fecha = new Date();
const diaDeLaSemana = fecha.getDay();
console.log(diaDeLaSemana); // Ejemplo de salida: 1 (lunes)
```

### getFullYear()
Devuelve el año.

```javascript
const fecha = new Date();
const año = fecha.getFullYear();
console.log(año); // Ejemplo de salida: 2024
```

### getHours()
Devuelve la hora (de 0 a 23).

```javascript
const fecha = new Date();
const hora = fecha.getHours();
console.log(hora); // Ejemplo de salida: 15
```

### getMilliseconds()
Devuelve los milisegundos (de 0 a 999).

```javascript
const fecha = new Date();
const milisegundos = fecha.getMilliseconds();
console.log(milisegundos); // Ejemplo de salida: 456
```

### getMinutes()
Devuelve los minutos (de 0 a 59).

```javascript
const fecha = new Date();
const minutos = fecha.getMinutes();
console.log(minutos); // Ejemplo de salida: 30
```

### getMonth()
Devuelve el mes (de 0 a 11).

```javascript
const fecha = new Date();
const mes = fecha.getMonth();
console.log(mes); // Ejemplo de salida: 1 (febrero)
```

### getSeconds()
Devuelve los segundos (de 0 a 59).

```javascript
const fecha = new Date();
const segundos = fecha.getSeconds();
console.log(segundos); // Ejemplo de salida: 45
```

### getTime()
Devuelve el número de milisegundos desde la medianoche del 1 de enero de 1970 hasta una fecha específica.

```javascript
const fecha = new Date();
const tiempoEnMilisegundos = fecha.getTime();
console.log(tiempoEnMilisegundos); // Ejemplo de salida: 1644831600000
```

### getTimezoneOffset()
Devuelve la diferencia de tiempo entre la hora UTC y la hora local, en minutos.

```javascript
const fecha = new Date();
const diferenciaDeZonaHoraria = fecha.getTimezoneOffset();
console.log(diferenciaDeZonaHoraria); // Ejemplo de salida: -300 (para UTC-5)
```

### getUTCDate()
Devuelve el día del mes según la hora universal (de 1 a 31).

```javascript
const fecha = new Date();
const diaDelMesUTC = fecha.getUTCDate();
console.log(diaDelMesUTC); // Ejemplo de salida: 13
```

### getUTCDay()
Devuelve el día de la semana según la hora universal (de 0 a 6).

```javascript
const fecha = new Date();
const diaDeLaSemanaUTC = fecha.getUTCDay();
console.log(diaDeLaSemanaUTC); // Ejemplo de salida: 1 (lunes)
```

### getUTCFullYear()
Devuelve el año según la hora universal.

```javascript
const fecha = new Date();
const añoUTC = fecha.getUTCFullYear();
console.log(añoUTC); // Ejemplo de salida: 2024
```

### getUTCHours()
Devuelve la hora según la hora universal (de 0 a 23).

```javascript
const fecha = new Date();
const horaUTC = fecha.getUTCHours();
console.log(horaUTC); // Ejemplo de salida: 20
```

### getUTCMilliseconds()
Devuelve los milisegundos según la hora universal (de 0 a 999).

```javascript
const fecha = new Date();
const milisegundosUTC = fecha.getUTCMilliseconds();
console.log(milisegundosUTC); // Ejemplo de salida: 456
```

### getUTCMinutes()
Devuelve los minutos según la hora universal (de 0 a 59).

```javascript
const fecha = new Date();
const minutosUTC = fecha.getUTCMinutes();
console.log(minutosUTC); // Ejemplo de salida: 30
```

### getUTCMonth()
Devuelve el mes según la hora universal (de 0 a 11).

```javascript
const fecha = new Date();
const mesUTC = fecha.getUTCMonth();
console.log(mesUTC); // Ejemplo de salida: 1 (febrero)
```

### getUTCSeconds()
Devuelve los segundos según la hora universal (de 0 a 59).

```javascript
const fecha = new Date();
const segundosUTC = fecha.getUTCSeconds();
console.log(segundosUTC); // Ejemplo de salida: 45
```

### getYear()
**Obsoleto.** Utilice el método `getFullYear()` en su lugar.

```javascript
const fecha = new Date();
const año = fecha.getYear();
console.log(año); // Ejemplo de salida: 124 (deprecado)
```

## Métodos de Configuración de Fechas

### now()
Devuelve el número de milisegundos desde la medianoche del 1 de enero de 1970.

```javascript
const tiempoActual = Date.now();
console.log(tiempoActual); // Ejemplo de salida: 1644831600000
```

### parse()
Analiza una cadena de fecha y devuelve el número de milisegundos desde el 1 de enero de 1970.

```javascript
const fechaString = "2024-02-13T15:30:00.000Z";
const tiempoDesde1970 = Date.parse(fechaString);
console.log(tiempoDesde1970); // Ejemplo de salida: 1644831600000
```

### prototype
Permite agregar propiedades y métodos a un objeto.

```javascript
Date.prototype.nuevoMetodo = function() {
  // Lógica del nuevo método
};

const fecha = new Date();
fecha.nuevoMetodo(); // Llamada al nuevo método
```

### setDate()
Establece el día del mes en un objeto de fecha.

```javascript
const fecha = new Date();
fecha.setDate(5);
console.log(fecha); // Ejemplo de salida:  Sun Feb 05 2024 15:30:00 GMT+0530 (hora estándar de India)
```

### setFullYear()
Establece el año en un objeto de fecha.

```javascript
const fecha = new Date();
fecha.setFullYear(2025);
console.log(fecha); // Ejemplo de salida:  Mon Feb 13 2025 15:30:00 GMT+0530 (hora estándar de India)
```

### setHours()
Establece la hora en un objeto de fecha.

```javascript
const fecha = new Date();


fecha.setHours(18);
console.log(fecha); // Ejemplo de salida:  Sun Feb 13 2024 18:30:00 GMT+0530 (hora estándar de India)
```

### setMilliseconds()
Establece los milisegundos en un objeto de fecha.

```javascript
const fecha = new Date();
fecha.setMilliseconds(500);
console.log(fecha); // Ejemplo de salida:  Sun Feb 13 2024 15:30:00 GMT+0530 (hora estándar de India) + 500 ms
```

### setMinutes()
Establece los minutos en un objeto de fecha.

```javascript
const fecha = new Date();
fecha.setMinutes(45);
console.log(fecha); // Ejemplo de salida:  Sun Feb 13 2024 15:45:00 GMT+0530 (hora estándar de India)
```

### setMonth()
Establece el mes en un objeto de fecha.

```javascript
const fecha = new Date();
fecha.setMonth(5);
console.log(fecha); // Ejemplo de salida:  Sat Jun 13 2024 15:30:00 GMT+0530 (hora estándar de India)
```

### setSeconds()
Establece los segundos en un objeto de fecha.

```javascript
const fecha = new Date();
fecha.setSeconds(20);
console.log(fecha); // Ejemplo de salida:  Sun Feb 13 2024 15:30:20 GMT+0530 (hora estándar de India)
```

### setTime()
Establece una fecha a un número específico de milisegundos después/antes del 1 de enero de 1970.

```javascript
const fecha = new Date();
fecha.setTime(1644835200000); // Establecer a las 2024-02-13 00:00:00 GMT
console.log(fecha);
```

### setUTCDate()
Establece el día del mes en un objeto de fecha, según la hora universal.

```javascript
const fecha = new Date();
fecha.setUTCDate(20);
console.log(fecha); // Ejemplo de salida:  Sun Feb 20 2024 15:30:00 GMT+0530 (hora estándar de India)
```

### setUTCFullYear()
Establece el año en un objeto de fecha, según la hora universal.

```javascript
const fecha = new Date();
fecha.setUTCFullYear(2023);
console.log(fecha); // Ejemplo de salida:  Mon Feb 13 2023 15:30:00 GMT+0530 (hora estándar de India)
```

### setUTCHours()
Establece la hora en un objeto de fecha, según la hora universal.

```javascript
const fecha = new Date();
fecha.setUTCHours(10);
console.log(fecha); // Ejemplo de salida:  Sun Feb 13 2024 10:30:00 GMT+0000 (UTC)
```

### setUTCMilliseconds()
Establece los milisegundos en un objeto de fecha, según la hora universal.

```javascript
const fecha = new Date();
fecha.setUTCMilliseconds(750);
console.log(fecha); // Ejemplo de salida:  Sun Feb 13 2024 15:30:00 GMT+0530 (hora estándar de India) + 750 ms
```

### setUTCMinutes()
Establece los minutos en un objeto de fecha, según la hora universal.

```javascript
const fecha = new Date();
fecha.setUTCMinutes(15);
console.log(fecha); // Ejemplo de salida:  Sun Feb 13 2024 15:15:00 GMT+0530 (hora estándar de India)
```

### setUTCMonth()
Establece el mes en un objeto de fecha, según la hora universal.

```javascript
const fecha = new Date();
fecha.setUTCMonth(8);
console.log(fecha); // Ejemplo de salida:  Thu Sep 13 2024 15:30:00 GMT+0530 (hora estándar de India)
```

### setUTCSeconds()
Establece los segundos en un objeto de fecha, según la hora universal.

```javascript
const fecha = new Date();
fecha.setUTCSeconds(40);
console.log(fecha); // Ejemplo de salida:  Sun Feb 13 2024 15:30:40 GMT+0530 (hora estándar de India)
```

### setYear()
**Obsoleto.** Utilice el método `setFullYear()` en su lugar.

```javascript
const fecha = new Date();
fecha.setYear(2025);
console.log(fecha); // Ejemplo de salida:  Mon Feb 13 2025 15:30:00 GMT+0530 (hora estándar de India)
```

## Métodos de Conversión a Cadena

### toDateString()
Convierte la porción de fecha de un objeto de fecha en una cadena legible.

```javascript
const fecha = new Date();
const cadenaFecha = fecha.toDateString();
console.log(cadenaFecha); // Ejemplo de salida:  Sun Feb 13 2024
```

### toGMTString()
**Obsoleto.** Utilice el método `toUTCString()` en su lugar.

```javascript
const fecha = new Date();
const cadenaGMT = fecha.toGMTString();
console.log(cadenaGMT); // Ejemplo de salida:  Sun, 13 Feb 2024 10:30:00 GMT
```

### toISOString()
Devuelve la fecha como una cadena, utilizando el formato ISO.

```javascript
const fecha = new Date();
const cadenaISO = fecha.toISOString();
console.log(cadenaISO); // Ejemplo de salida:  2024-02-13T10:30:00.000Z
```

### toJSON()
Devuelve la fecha como una cadena en formato JSON.

```javascript
const fecha = new Date();
const cadenaJSON = fecha.toJSON();
console.log(cadenaJSON); // Ejemplo de salida:  2024-02-13T10:30:00.000Z
```

### toLocaleDateString()
Devuelve la porción de fecha de un objeto de fecha como una cadena, utilizando las convenciones locales.

```javascript
const fecha = new Date();
const cadenaLocalFecha = fecha.toLocaleDateString();
console.log(cadenaLocalFecha); // Ejemplo de salida:  13/02/2024 (dependiendo de la configuración regional)
```

### toLocaleTimeString()
Devuelve la porción de tiempo de un objeto de fecha como una cadena, utilizando las convenciones locales.

```javascript
const fecha = new Date();
const cadenaLocalTiempo = fecha.toLocaleTimeString();
console.log(cadenaLocalTiempo); // Ejemplo de salida:  15:30:00 (dependiendo de la configuración regional)
```

### toLocaleString()
Convierte un objeto de fecha a una cadena, utilizando las convenciones locales.

```javascript
const fecha = new Date();
const cadenaLocal = fecha.toLocaleString();
console.log(cadenaLocal); // Ejemplo de salida:  13/02/2024, 15:30:00 (dependiendo de la configuración regional)
``

`

### toString()
Convierte un objeto de fecha a una cadena.

```javascript
const fecha = new Date();
const cadenaCompleta = fecha.toString();
console.log(cadenaCompleta); // Ejemplo de salida:  Sun Feb 13 2024 15:30:00 GMT+0530 (hora estándar de India)
```

### toTimeString()
Convierte la porción de tiempo de un objeto de fecha a una cadena.

```javascript
const fecha = new Date();
const cadenaTiempo = fecha.toTimeString();
console.log(cadenaTiempo); // Ejemplo de salida:  15:30:00 GMT+0530 (hora estándar de India)
```

### toUTCString()
Convierte un objeto de fecha a una cadena, según la hora universal.

```javascript
const fecha = new Date();
const cadenaUTC = fecha.toUTCString();
console.log(cadenaUTC); // Ejemplo de salida:  Sun, 13 Feb 2024 10:30:00 GMT
```

## Otros Métodos

### UTC()
Devuelve el número de milisegundos en una fecha desde la medianoche del 1 de enero de 1970, según la hora universal.

```javascript
const fecha = new Date();
const tiempoEnUTC = Date.UTC(2024, 1, 13, 12, 30, 0);
console.log(tiempoEnUTC); // Ejemplo de salida: 1644838800000
```

### valueOf()
Devuelve el valor primitivo de un objeto de fecha.

```javascript
const fecha = new Date();
const valorPrimitivo = fecha.valueOf();
console.log(valorPrimitivo); // Ejemplo de salida: 1644831600000
```

¡Gracias por utilizar estos métodos del objeto `Date` en JavaScript! Si tienes alguna pregunta o comentario, no dudes en contactarnos.
