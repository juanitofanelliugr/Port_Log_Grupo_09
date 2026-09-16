# Conclusión

El análisis realizado permitió observar que el dataset heredado presentaba varios problemas de calidad. Durante el proceso se descartó un 70,20% de los registros, considerando tanto la limpieza como la selección final de las infracciones. Entre los principales problemas encontrados se observaron valores nulos, fechas y horas inválidas, formatos inconsistentes y valores atípicos. Además, dentro de las infracciones analizadas, un 6,49% tenía fecha inválida y un 5,82% hora inválida.

Respecto a los patrones detectados, el turno con mayor cantidad de infracciones fue la Tarde, con 124, seguido muy de cerca por Madrugada, con 123. Los muelles con mayor cantidad fueron MUELLE-B y MUELLE-D, con 79 infracciones cada uno. En cuanto al tipo de carga, TRIGO fue el más frecuente, representando el 15,44% de las infracciones.

Incorporar los datos originales al nuevo sistema sin realizar una limpieza previa podría generar resultados incorrectos y análisis poco confiables, debido a la presencia de datos faltantes, formatos inválidos y valores atípicos.

Como mejora para el proceso de captura de datos del puerto, se podrían implementar validaciones automáticas al momento de ingresar la información, controlando el formato de fechas y horas, evitando campos obligatorios vacíos y verificando que valores como la velocidad y el tonelaje estén dentro de rangos válidos. Esto permitiría detectar errores desde el momento de la carga y mejorar la calidad de los datos.
