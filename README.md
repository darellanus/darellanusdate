#darellanus Date
Un autilidad para manejar fechas en formato timestamp y long time

#install

```bash
npm install darellanusdate
```
#Funciones utilizadas
getTimeStamp() --> funcion que muestra el tiempo en un instante dado
getLongTime(idioma-region) --> funcion que muestra el tiempo en un idioma especificado y con un formato especificado.

function getTimestamp() {
  return Date.now();
}

function getLongTime(locale = "es-ES") {
  const options = {
    weekday: "long",
    year: "numeric",
    month: "long",
    day: "numeric",
    hour: "numeric",
    minute: "numeric",
    second: "numeric",
    timeZoneName: "short",
  };
  return new Date().toLocaleString(locale, options);
}
