La cadena de gimnasios Model Fitness está desarrollando una estrategia de interacción con clientes basada en datos analíticos.
Uno de los problemas más comunes que enfrentan los gimnasios y otros servicios es la pérdida de clientes.Sin embargo, a veces no es obvio que un cliente se haya ido: puede que se vaya de puntillas.

Los indicadores de pérdida varían de un campo a otro.
Si un usuario o una usuaria compra en una tienda en línea con poca frecuencia, pero con regularidad, no se puede decir que ha huido.
Pero si durante dos semanas no ha abierto un canal que se actualiza a diario, es motivo de preocupación,es posible que tu seguidor o seguidora se haya aburrido y te haya abandonado.
En el caso de un gimnasio, tiene sentido decir que un cliente se ha ido si no viene durante un mes. 
Por supuesto, es posible que estén en Cancún y retomen sus visitas cuando regresen, pero ese no es un caso típico. Por lo general, si un/a cliente se une, viene varias veces y luego desaparece, es poco probable que regrese.

Con el fin de combatir la cancelación, Model Fitness ha digitalizado varios de sus perfiles de clientes.
Este proyecto consiste en analizarlos y elaborar una estrategia de retención de clientes.

los datos usados son los siguentes:

'Churn' — la cancelación para el mes en cuestión
'gender'.
'Near_Location' — si el/la usuario/a vive o trabaja en el vecindario donde se encuentra el gimnasio.
'Partner' — si el/la usuario/a trabaja en una compañía asociada (el gimnasio tiene empresas asociadas cuyos empleados obtienen descuentos; en esos casos el gimnasio almacena información sobre los empleadores de los clientes).
'Promo_friends' — si el/la usuario/a originalmente se inscribió mediante una oferta “trae a un/a amigo/a” (se utilizó el código promocional de un/a amigo/a cuando pagaron el primer abono).
'Phone' — si el/la usuario/a aportó el número de teléfono.
'Age'.
'Lifetime' — el tiempo (en meses) desde que el/la usuario/a llegó por primera vez al gimnasio.
Datos del registro de visitas y compras y datos sobre el estado actual de la membresía:
'Contract_period' — 1 mes, 3 meses, 6 meses o 1 año.
'Month_to_end_contract' — los meses que faltan hasta que expire el contrato.
'Group_visits' — si el/la usuario/a participa en sesiones grupales.
'Avg_class_frequency_total' — frecuencia media de visitas por semana a lo largo de la vida del cliente.
'Avg_class_frequency_current_month' — frecuencia media de visitas por semana durante el mes en curso.
'Avg_additional_charges_total' — cantidad total de dinero gastado en otros servicios del gimnasio: cafetería, productos deportivos, cosméticos, masajes, etc.

Como todo proyecto estos llevan pasos y etapas comenzando con:
1.-El análisis exploratorio de datos (EDA)
Objetivos: ¿contiene alguna característica ausente? Estudia los valores promedio y la desviación estándar.
Observar los valores medios de las características en dos grupos.
Trazar histogramas de barras y distribuciones de características para aquellas personas que se fueron (cancelación) y para las que se quedaron.
Crear una matriz de correlación.

2.-Construir un modelo para predecir la cancelación de usuarios
Crea un modelo de clasificación binaria para clientes donde la característica objetivo es la marcha del usuario o la usuaria el mes siguiente.
Objetivos: Evalúar la exactitud, precisión y recall para ambos modelos utilizando los datos de validación. Utilízalos para comparar los modelos. ¿Qué modelo dio mejores resultados?

3.-Crear clústeres de usuarios
Se utiliza la función linkage() para crear una matriz de distancias basada en la matriz de características estandarizada y trazar un dendrograma.
Objetivos: Utilizar el gráfico (dendrograma) resultante para estimar el número de clústeres que puedes destacar.
Entrena el modelo de clustering con el algortimo K-means y predice los clústeres de clientes.
Calcular la tasa de cancelación para cada clúster. 
¿Difieren en términos de tasa de cancelación? ¿Qué grupos son propensos a irse y cuáles son leales?

4.- Sacar conclusiones y hacer recomendaciones básicas con respecto a la estrategia para la interacción y retención de clientes.
