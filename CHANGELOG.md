### Ejercicio 03 - Modelo lógico de datos

- Diseño del modelo lógico de Buque, Movimiento, Radar y Evidencia.
- Definición de atributos, claves primarias, claves foráneas y cardinalidades.
- Consideración del radar móvil, que puede registrar movimientos en distintos muelles.
- Representación del muelle como atributo de Movimiento.

## Sprint 3

### Día 2 - Migración de imágenes a DVC

- Migración de 100 imágenes de `port_log/data/raw/imgs` a DVC.
- Creación del archivo de seguimiento `imgs.dvc`.
- Configuración de Supabase S3 como almacenamiento remoto.
- Sincronización de imágenes mediante DVC.



### Día 1 - Inicio del Sprint 3

- Creación de la rama `Sprint_3` desde `Sprint_2`.
- Configuración del entorno de trabajo en Google Colab.
- Verificación de la conexión con GitHub.
- Instalación y configuración inicial de DVC.
- Verificación de los cuatro datasets anteriores.
- Comprobación de registros y fechas de modificación.
- Actualización de README y CHANGELOG.

# CHANGELOG

[Ejercicio 6 - Día 2]

- Se analizaron los resultados del OCR y del matching de matrículas.
- Se identificó que 414 de las 447 infracciones corresponden a buques con imágenes asociadas a su matrícula.
- Se aclaró que la asociación por matrícula no permite validar visualmente una infracción individual.
- Se compararon las tasas de coincidencia de los grupos plates y completes.
- Se analizaron las posibles dificultades del OCR relacionadas con iluminación, desenfoque y distancia.
- Se propusieron mejoras en la captura de imágenes, el preprocesamiento y el algoritmo de matching.
- Se destacó la importancia de registrar el movimiento_id, la fecha y la hora para vincular imágenes con movimientos específicos.

[Ejercicio 5 - Día 2]

- Se analizaron las infracciones de velocidad con y sin imágenes asociadas.
- Se identificaron 414 infracciones vinculadas a matrículas con imágenes disponibles y 33 sin imágenes asociadas.
- Se calcularon las infracciones pendientes sin imágenes asociadas, obteniendo un total de 6.
- Se contabilizaron 95 imágenes con match y 5 sin coincidencia.
- Se calculó el ratio promedio de similitud de las imágenes coincidentes.
- Se compararon las tasas de matching entre los grupos plates y completes.
- Se corrigió el conteo de imágenes para evitar duplicaciones por matrícula.
- Se diferenció la asociación de imágenes a buques de la evidencia visual de una infracción específica.

[Ejercicio 4 - Día 2]

- Se implementó la extracción automática de matrículas mediante EasyOCR.
- Se optimizó el procesamiento cargando el lector OCR una sola vez.
- Se normalizaron las matrículas detectadas y las del dataset.
- Se calculó el porcentaje de similitud mediante SequenceMatcher.
- Se estableció un umbral mínimo de coincidencia del 75%.
- Se identificaron 95 imágenes coincidentes, correspondientes a 19 matrículas diferentes.
- Se diferenciaron las imágenes coincidentes de los movimientos asociados a cada matrícula.
- Se evitó asignar arbitrariamente una imagen a un movimiento individual.
- Se actualizó group_images.json con las matrículas detectadas, las coincidencias y sus ratios.
- Se generó port_movements_image.csv conservando los 447 movimientos originales.
- Se incorporaron las imágenes, matrículas OCR, ratios y grupos asociados a cada buque.
- Se conservaron los movimientos sin imágenes asociadas.

[Ejercicio 3 - Día 2]

- Se procesaron las imágenes de los grupos plates y completes.
- Se convirtieron las imágenes a escala de grises utilizando OpenCV.
- Se aplicó ecualización de histogramas para mejorar el contraste.
- Se realizó un suavizado gaussiano para reducir el ruido.
- Se aplicó el detector de bordes Canny sobre las imágenes suavizadas.
- Se guardaron las imágenes procesadas en las carpetas correspondientes dentro de data/interim/imgs.
- Se reemplazó el uso de PIL por OpenCV según las correcciones del docente.

[Ejercicio 2 - Día 2]

- Se clasificaron las 100 imágenes del dataset en los grupos plates y completes.
- Se utilizó el nombre de los archivos para identificar cada tipo de imagen.
- Se construyó el diccionario group_images con los datos principales de las imágenes.
- Se registraron el nombre, ancho, alto, área, ruta y matrícula de cada imagen.
- Se guardó la información en port_log/data/interim/group_images.json.

[Ejercicio 1 - Día 2]

- Se creó la rama Sprint_2 a partir de Sprint_1.
- Se descargaron y organizaron 100 imágenes en data/raw/imgs.
- Se verificó la disponibilidad de los archivos CSV.
- Se comprobaron 1500 registros raw, 447 interim y 8 summary.
- Se actualizó el README con la descripción del Sprint 2.

[Ejercicio 7]

- Se realizó la conclusión sobre la calidad de los datos, los patrones de infracción, el impacto de la falta de limpieza y las propuestas de mejora.

[Ejercicio 6]

- Se respondieron las preguntas de negocio calculando porcentajes de error, cargas frecuentes y duración de estadía.

[Ejercicio 5]

- Se graficaron las 10 matrículas con más infracciones.
- Se graficó la distribución de infracciones por turno del día.
- Se graficó el total de infracciones por mes.
- Se generó el histograma del exceso de velocidad real con curva KDE.
- Se graficó el exceso de velocidad promedio por muelle.
- Se compararon las infracciones con fecha válida e inválida.
- Se exportaron los gráficos en data/interim/plots.

[Ejercicio 4]

- Se definió la clase PortAnalyzer para analizar el DataFrame limpio.
- Se implementó el ranking de matrículas con más infracciones.
- Se agruparon las infracciones por turno, muelle y tipo de carga.
- Se calcularon los excesos de velocidad promedio real y con tolerancia.
- Se creó un objeto PortAnalyzer y se invocaron sus métodos en celdas separadas.

[Ejercicio 3]

- Se normalizaron las fechas y horas de ingreso y egreso.
- Se calculó la duración de cada movimiento portuario.
- Se normalizaron las matrículas y los muelles.
- Se eliminaron registros con datos nulos en columnas críticas.
- Se detectaron y eliminaron outliers mediante el método IQR.
- Se calcularon los excesos de velocidad reales y con 5% de tolerancia.
- Se conservaron únicamente los movimientos con infracción de velocidad.
- Se generó el dataset limpio en data/interim.
- Se exportó el resumen estadístico del Sprint 1 en reports.

[Ejercicio 2]

- Se descargó y almacenó el dataset raw.
- Se visualizaron las primeras y últimas 5 filas.
- Se analizaron los tipos de datos y las columnas que requieren conversión.
- Se contabilizaron los valores nulos.
- Se calculó el porcentaje de valores correctos por columna.

[Ejercicio 1]

- Se inicializó y configuró Git.
- Se creó la rama Sprint_1.
- Se creó la estructura de directorios del proyecto.
