# Universal_and_DisneyWorld_Incident_Data_2002-2022

Este proyecto tuvo como objetivo analizar los incidentes ocurridos en los parques de atracciones de Universal y Disney World entre los años 2002 y 2022.

## Conjunto de Datos:
Encontramos las siguientes columnas en los datos iniciales:
- Company: Universal o Disney World
- Incident_date: Fecha del suceso
- Ride_name_dirty: Nombre de la atracción en sucio
- Ride_name: Nombre de la atracción en limpio
- Theme_Park: Parque dentro del que sucede el incidente
- age_gender: Recoge tanto la edad como el género
- description: Descripción de en qué consistió el incidente

## Retoque de características:
Se ha trabajado con los datos iniciales:
- dividiendolos (como es el caso de age_gender o como en la fecha creando características separadas para el día, día de la semana, mes, año), 
- creando categorias (en el caso de la edad), 
- creando nuevas columnas que indican si un incidente ocurre o no:
    * 'sickness ind' - mareos 
    * 'physical pain ind' - dolor físico
    * 'chest problem ind' - problemas relacionados con el corazón
    * 'seizure ind' - convulsiones
    * 'unconscious ind' - pérdida de consciencia
    * 'known condition ind' - condición médica previamente conocida por el individuo
    * 'hospital ind' - visita al hospital
    * 'deceased ind' - fallecimientos


# Análisis de correlación
Algunas correlaciones interesantes encontradas fueron las siguientes:
- Los niños pequeños tienen un indicador de hospitalización más alto que cualquier otro grupo de edad. Esto podría deberse a su edad y a la precaución de evitar cualquier riesgo.
- Mirando de cerca las correlaciones entre las visitas al hospital y otras variables encontramos una correlación fuerte con los fallecimientos y débil con la pérdida de conciencia. 
- Las lesiones físicas se producen más en las atracciones familiares. Seguidos de montañas rusas y atracciones emocionantes y, por último, las atracciones acuáticas.
- Los paseos familiares y las personas mayores de 60 años no son una buena combinación; estos dos campos muestran una correlación bastante alta, lo que indica que los incidentes ocurren con bastante frecuencia. Sería interesante ver qué tipo de atracciones son las más usadas por rango de edad.
- Las condiciones preexistentes muestran una correlación bastante alta con el año del incidente. Podría deberse a que ha empezado a registrase ese dato más recientemente.
- En general, no vemos correlaciones muy fuerte, pero el tamaño de datos es relativamente pequeño, por lo que esto debe tenerse en cuenta al hacer estas suposiciones.