# ANALISIS-ESTADISCO
 Desarrollo de un estudio analítico sobre 500 clientes para evaluar el rendimiento financiero de las tarifas Surf y Ultimate. Se aplicaron técnicas estadísticas y pruebas de hipótesis para determinar la estrategia comercial óptima basada en el comportamiento de uso (llamadas, mensajes, etc.).
Conclusión general
[En esta sección final, enumera tus conclusiones importantes. Asegúrate de que estas abarquen todas las decisiones (suposiciones) importantes que adoptaste y que determinaron la forma elegida para procesar y analizar los datos.]

En este proyecto, realizamos un análisis exhaustivo de los planes de prepago Surf y Ultimate ofrecidos por Megaline para determinar cuál de ellos genera más ingresos. A continuación, se enumeran las conclusiones y decisiones clave que determinaron la forma en que procesamos y analizamos los datos:

# Preparación y Limpieza de Datos:

Conversión de Fechas: Convertimos las fechas en objetos datetime para facilitar el análisis basado en el tiempo de los dataframe, internet, mensajes y llamadas.

Creación de Columnas de Mes: Añadimos columnas que representan el mes para permitir la agrupación mensual de los datos.

Cálculo del Uso Total:

Agrupamos los datos de llamadas, mensajes y uso de datos por usuario y mes para obtener el total de minutos utilizados, SMS enviados y datos consumidos.

Unión de Datos:

Unimos los datos de llamadas, mensajes e internet con los datos de usuarios para tener un conjunto de datos completo que incluya la información del plan, el uso de servicios y las tarifas correspondientes, tambien añadimos el plan, obteniendo un dateframe grande con toda la informacion procesada.

Cálculo de Ingresos:

Desarrollamos una función para calcular los ingresos totales por usuario, considerando tanto los ingresos básicos por suscripción mensual como los ingresos adicionales por exceder los límites del plan.

Distribucion en grafico: Graficamos la distribucion por mes de llamadas, mensajes, internet y planes.

Análisis Estadístico:

Formulación de Hipótesis del dataframe:

Hipótesis Nula (H0): Los ingresos promedio de los usuarios del plan Ultimate son iguales a los ingresos promedio de los usuarios del plan Surf.

Hipótesis Alternativa (H1): Los ingresos promedio de los usuarios del plan Ultimate son diferentes a los ingresos promedio de los usuarios del plan Surf.

Selección de Prueba Estadística: Usamos una prueba t de dos muestras (independiente) para comparar las medias de ingresos de los dos planes.

Establecimos un nivel de significancia de 0.05 para la prueba estadística.

Resultados: El valor p obtenido 2.2734565113013996e-25 fue extremadamente bajo, permitiéndonos rechazar la hipótesis nula y concluir que hay una diferencia significativa en los ingresos promedio entre los planes Ultimate y Surf.

Formulación de Hipótesis de la ciudades:

Hipótesis Nula (H0): Los ingresos promedio de los usuarios en NY-NJ son iguales a los ingresos promedio de los usuarios del resto de cuidades.

Hipótesis Alternativa (H1): Los ingresos promedio de los usuarios en NY-NJ son diferentes a los ingresos promedio de los usuarios del resto de cuidades.

Selección de Prueba Estadística: Usamos una prueba t de dos muestras (independiente) para comparar las medias de ingresos de las cuidades (NY-NJ) con el resto de estados.

Establecimos un nivel de significancia de 0.05 para la prueba estadística.

Resultados: El valor p obtenido 0.02562213042590581 fue extremadamente bajo, permitiéndonos rechazar la hipótesis nula y concluir que hay una diferencia significativa en los ingresos promedio entre las ciudades de NY-NJ y el resto de estados.

CONCLUSIONES IMPORTANTES:

Diferencia Significativa en los Ingresos Promedio:

Los resultados de la prueba t indicaron una diferencia significativa en los ingresos promedio entre los usuarios de los planes Ultimate y Surf. Específicamente, el plan Ultimate genera más ingresos promedio que el plan Surf.

Beneficios del Plan Ultimate:

Aunque el plan Ultimate tiene una tarifa de suscripción más alta, ofrece más minutos, mensajes y datos incluidos, lo que resulta en menos cargos adicionales para los usuarios y, en general, mayores ingresos para la empresa.

Consideraciones para la Toma de Decisiones:

Estos hallazgos pueden informar las decisiones del departamento comercial de Megaline, especialmente en lo que respecta a la asignación del presupuesto de publicidad y el enfoque de marketing para maximizar los ingresos.
