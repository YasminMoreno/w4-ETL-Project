# W4-proyecto-ETL

Proyecto ETL sobre extracción, transformación y carga.

## Introducción

Para este proyecto de extracción, transformación y carga vamos a buscar información en diferentes páginas webs sobre como afecta el clima y el área geográfica en los que han sido los `top nº1` en `10 países`diferentes. 

Para ello vamos a utiplizar python, web scraping y MySQL Workbench. 

Posteriormente crearemos unas preguntas y las contestaremos mediante queries para obtener la respuesta a la información que buscamos.
 
 
## Objetivos

1. Hacer el proyecto ETL ( extraer datos, transformarlos, limpiarlos y cargarlos en una base de datos).
2. Usar 3 fuentes y 2 métodos.
3. Hacer limìeza con python y cargarlo en SQL.
4. Hacer las preguntas a las cuales queremos contestar.
5. Utilizar las queries para resolver estas preguntas.


## Procedimiento

1. Preparamos la idea que vamos a desarrollar. En este caso vamos a descubrir cuales son las canciones mas escuchadas en diferentes países y compararlo con área gegráfica y clima del lugar.  
2. Extraemos varios csv de la web `https://charts.spotify.com/home` en total 10 países para crear la tabla `top_mundial_spotify`.
3. Extraemos mediante web scraping con BeautifulSoup de la web `https://catking.in/list-of-countries-capitals-currencies-of-the-world/` para hacer la tabla de `countries`las diferentes capitales y píases del mundo. 
4. Extraemos la tercera fuente mediante web scraping con BeautifulSoup de la web `https://www.aerisweather.com/weather` para crear la tabla `weather`.
5.Limpiamos en diferentes jupyters cada una de las tablas que queremos hacer.
6.hacemos una cuarta tabla llamada `countryweather` para posteriormente poder unir countries y weather.
7. Exportamos todos los csv convertidos a xls a MySQL Workbench y creamos el database `spotiweather` con sus Primeray Keys y Foreing Keys. Todo ello creado mediante python,  por si en un futuro queremos rectificar alguna tabla para que nos sea más sencillo a la hora de ejecutar.
8. Una vez exportado el database creamos la EER.
