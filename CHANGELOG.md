# CHANGELOG

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

[Ejercicio 7]

- Se realizó la conclusión sobre la calidad de los datos, los patrones de infracción, el impacto de la falta de limpieza y las propuestas de mejora.

[Ejercicio 7]

- Se realizó la conclusión sobre la calidad de los datos, los patrones de infracción, el impacto de la falta de limpieza y las propuestas de mejora.

[Ejercicio 7]

- Se realizó la conclusión sobre la calidad de los datos, los patrones de infracción, el impacto de la falta de limpieza y las propuestas de mejora.

[Ejercicio 7]

- Se realizó la conclusión sobre la calidad de los datos, los patrones de infracción, el impacto de la falta de limpieza y las propuestas de mejora.

[Ejercicio 7]

- Se realizó la conclusión sobre la calidad de los datos, los patrones de infracción, el impacto de la falta de limpieza y las propuestas de mejora.

[Ejercicio 7]

- Se realizó la conclusión sobre la calidad de los datos, los patrones de infracción, el impacto de la falta de limpieza y las propuestas de mejora.

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
