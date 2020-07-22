# Guillermo Hilal 88/100
## 1) Plantear una pregunta que quieran responder con estos datos: 20/20
Introduce bien a las bandas que vas a usar. Hubiera estado genial que usaras más canciones o grupos para la competencia, pero tu justificación para reducir el volumen me parece válida, sumado a que no hay muchas canciones de Bándalos Chinos en Spotify. La elección y descripción de features me parece muy buena, se nota que tenés conocimientos sobre música.
## 2) Obtener datos para responder la pregunta: 18/20
El código cumple con la utilidad exigida, está bien estructurado y es fácil de leer. LosDataFrames están bien generados y organizados. 
### Errores:
- En set_and_save_dataframe no se respeta el estilo en instrucciones que abarcan más de una línea(-2).
### Warnings:
- Para features categóricas como key y mode es mejor usar encodings en vez de valores textuales (en este caso se da que vienen encodeadas ya, así que no era necesario pasarlas a string).
- Evitar hardcodear, en este caso no hay problema porque son sólo dos bandas, pero tener en cuenta que puede darse que en otro trabajo sean muchas más y quedaría feo una celda con 30 ids hardcodeados.

## 3) Hacer un gráfico de estilo radar chart comparando a su artista o banda con 'la competencia': 20/30

### Errores: 
No se calculan los estadísticos para key y beat, esto tiene que ver con lo que aclaro en el primer warning del ejercicio 2). Si hubieras dejado los valores numéricos podrías haberlas calculado la media y mediana y reescalado los valores (acá también entran duration y loudness) para el boxplot (-20).
No se usó radar chart, sin embargo el boxplot utiliza los valores estadísticos requeridos y capta los outliers y la desviación estándar (aunque me hubiera gustado que lo justifiques con estos argumentos). Los gráficos de barras y de correlación junto con sus análisis son un plus que compensa parcialmente el error(+10).

## 4) Escribir un informe: 30/30
Excelente la argumentación. Importante que hayas aclarado que hay otros factores fuera de lo musical que influyen.

------------------------------

# Ivan Gutiérrez 91/100

## 1) Plantear una pregunta que quieran responder con estos datos: 13/20
Está bien, pero la idea era que eligieran ustedes algún conjunto de artistas o un género. En este caso vos lo hiciste con la playlist que vamos a usar desde el práctico 3 en adelante, lo  cual es bueno por el volumen de datos que manejas, pero deberías haber aclarado esto en tu pregunta escribiendo, por ejemplo, ¿Cuales son los 5 generos más destacados de la playlist colaborativa para la mentoría? ¿Qué hace que el cuarteto destaque sobre los demás? Porque por más que las respuestas estén bien, si no responden a lo que preguntás vas a tener problemas (-7).
Fuera de eso me pareció interesante que experimentaras con esta playlist de cara al trabajo que vamos a hacer en el futuro.

## 2) Obtener datos para responder la pregunta: 19/20
El código cumple con la utilidad exigida, está bien estructurado y es fácil de leer. Los DataFrame están bien generados y organizados. Hacés un buen uso de las funciones de pandas. Los gráficos de barras y boxplots ayudan a la comprensión de la conformación del conjunto de datos. Es importante que hayas obtenido además datos adicionales dentro del género cuarteto para comparar a los artistas del género(+1).
### Errores:
- En loadArtistGenre  en la primera línea hay un comentario vacío.(-1)
-En loadTracksFromPlayListItems dejás una linea en blanco al principio, esto no corresponde con el estilo de las demás funciones.(-1)

## 3) Hacer un gráfico de estilo radar chart comparando a su artista o banda con 'la competencia': 25/30
### Warnings: 
En tu conjunto de datos se observa que los valores para la feature instrumentalness son muy chiquitos, para mejorar un poco el gráfico podrías haberlos reescalado para que tomen valores entre 0 y 1 y así hacer un poco más apreciables las diferencias entre géneros y entre artistas de cuarteto.

Solucionando este warning podrías haber incluído a tempo entre las features del gráfico. (-5)

## 4) Escribir un informe: 30/30
Algunos errores de markdown (saltos de línea deberían ser dobles entre párrafos). Fuera de eso está bien, explica el desarrollo del proyecto y los datos que utilizaste.

------------------------------

# Damián Campana 90/100

## 1) Plantear una pregunta que quieran responder con estos datos: 20/20
Al principio me parecieron raras las preguntas que planteaste, pero después de leer la conclusión y de ver los análisis que hiciste me pareció una propuesta muy interesante, ya que cuestionás la falsa premisa en la que basamos este práctico (sólo las features musicales cuentan para medir el éxito de una canción).

## 2) Obtener datos para responder la pregunta: 15/20
El código cumple con la utilidad exigida. El DataFrame están bien generados y organizados. Muy bien el chequeo de valores nulos!(+4) También me parece bien que hayas introducido la feature key, siendo que es menos intuitiva que las demás, que hayas hecho gráficos y que hayas usado la feature popularity(+3). 
### Errores:
- No sos consistente en tu estilo de código, hay veces en que dejás una o dos líneas aleatoriamente entre “grupos” de instrucciones. (-5) 
- Hardcodeo en la celda [4], acá no molesta tanto, pero pensá que en un dataset más grande va a dificultar leer tu trabajo. (-2)
- Dejás varias instrucciones comentadas, salvo que estuvieran como opción las líneas al correr el programa, es mala práctica hacer esto. (-3)
- Celda [30]: no lo comentes, es fundamental que sea reproducible! (-2)

## 3) Hacer un gráfico de estilo radar chart comparando a su artista o banda con 'la competencia': 25/30
El gráfico está perfecto, mostrás primero los valores y luego el gráfico se corresponde a estos.

Solucionando este warning podrías haber incluído a tempo entre las features del gráfico. (-5)

## 4) Escribir un informe: 30/30
Excelente la argumentación. Fundamental que hayas propuesto que hay otros factores fuera de lo musical que influyen.

------------------------------

#Daniel Cattaneo 100/100

## 1) Plantear una pregunta que quieran responder con estos datos: 20/20
Me pareció muy interesante que hayas hecho un recorrido por la trayectoria de los Beatles a lo largo de su (corta) existencia. Creo que un análisis de este estilo se puede aplicar en un montón de contextos y nos ayuda a entender al desarrollo de los artistas y su estilo.

## 2) Obtener datos para responder la pregunta: 20/20
El código es simple, cumple con la utilidad exigida y está impecable en cuanto a estilo. Muy bien pensados los filtros que usaste para los álbumes. 

## 3) Hacer un gráfico de estilo radar chart comparando a su artista o banda con 'la competencia': 25/30
El gráfico está perfecto para entender la variación a lo largo del tiempo de los valores medios en las features que elegiste, siendo esto mejor visualizado con el gráfico que elegiste vs los radar charts. El único punto en contra fue que me hubiera gustado leer esta justificación de tu parte al no elegir el radar chart (-5).

## 4) Escribir un informe: 40/30
El informe es excelente. No solo profundiza los puntos que pueden quedar sueltos o incompletos de las consignas anteriores, sino que además citás artículos con trabajos similares y describís tu motivación a la hora de realizar el trabajo. Muy bien descritos los resultados obtenidos y el análisis de los gráficos (+10).

------------------------------

# Karen Palacio 93/100
## 1) Plantear una pregunta que quieran responder con estos datos: 15/20
Muy bien. Solemos asumir los valores de las features de Spotify y los criterios en que se basan como algo absoluto. Me parece buena tu intención de cuestionar esto. 
### Errores:
- Hubiera estado bueno que introdujeras un poco mejor qué es la música experimental para que leer el trabajo no requiriera fuentes adicionales (-5).

## 2) Obtener datos para responder la pregunta: 15/20
El código cumple con la utilidad exigida. El DataFrame están bien generados y organizados. Los gráficos de las distribuciones de los artistas y las features ayudan a la comprensión de tu conjunto de datos. El volumen de datos utilizados es grande y sirve más para respaldar tus resultados.
### Errores:
- En el código de los gráficos no se respeta el estilo en instrucciones que abarcan más de una línea(máximo 80 caracteres por línea) (-5).

## 3) Hacer un gráfico de estilo radar chart comparando a su artista o banda con 'la competencia': 28/30
El gráfico está perfecto, mostrás primero los valores y luego el gráfico se corresponde a estos.

### Errores:
- We can see that given a random song of the dataset, there's a high probability that the song will rank above average in the danceability score, meaning it's probably considered as rhythmically stable, with strong beats and present an overall regularity. Esto no es tan así, si chequeás el gráfico de distribución de las features arriba de esta afirmación se puede ver que si bien es bastante pareja la distribución de danceability, hay más canciones con valores bajos para la feature (-2). 

### 4) Escribir un informe: 35/30
Excelente, principalmente porque demostrás tu punto. Las observaciones y el análisis de casos particulares aportan mucho al informe, ya que muestran errores por parte del algoritmo que anota las features de Spotify(+5). También es bueno que hables de trabajo futuro.

------------------------------

# Adrián Lucero 100/100

## 1) Plantear una pregunta que quieran responder con estos datos: 25/20
Una elección completa y bien planteada. Es muy interesante que primero compares los discos de un mismo grupo y luego con otra banda. Además elegís dos preguntas para responder (+5).

## 2) Obtener datos para responder la pregunta: 18/20
El código cumple con la utilidad exigida, está bien estructurado, es muy prolijo y es fácil de leer. Los DataFrames están bien generados y organizados. Los análisis disco a disco están muy bien.
### Errores:
Comentarios multilínea en la celda [4] deberían ir entre triple quotes """ """ (-2).
Múltiples instrucciones de más de 80 caracteres en una sola línea (-3).
### Warnings:
Guarda con los hardcodeos en [4]!

## 3) Hacer un gráfico de estilo radar chart comparando a su artista o banda con 'la competencia': 30/30
El gráfico está perfecto, mostrás primero los valores y luego el gráfico se corresponde a estos.

## 4) Escribir un informe: 35/30
Excelente informe. Los gráficos extra, los análisis de correlación y los datos sobre los discos que analizás ayudan a la comprensión del conjunto de datos (+5).
