# Pr-ctica-Data-Analytics-V3-Unidad-4-Dashboard-An-lisis-de-Datos-Google-Sheets
Práctica de la unidad 4 Dashboard &amp; Análisis de Datos Google Sheets del curso Data &amp; Analytics V3
El objetivo de este proyecto es realizar un análisis exploratorio de datos y representarlo mediante un dashboard interactivo, utilizando Excel / Google Sheets.

## 1.Estructura del proyecto
Enlace Google Sheets - Enlace al archivo con el ejercico
Proyecto unidad 4.xlsx - Copia del ejercicio en .xlsx
README.md
StudentPerformanceFactors BRUTO.csv - Datos en bruto, tal cual descargados

## 2.Origen de los datos
El conjunto de datos utilizado en este proyecto corresponde a un dataset sobre factores que influyen en el rendimiento académico de los estudiantes.
Consta de 6.607 filas y 20 columnas

- Plataforma: Kaggle  
- Nombre del dataset: Student Performance Factors  
- Enlace: https://www.kaggle.com/datasets/lainguyn123/student-performance-factors

## 3. Análisis descriptivo de los datos
- Hours_Studied: Media de horas que ha estudiado cada alumno por semana
- Attendance: Porcentaje de clases asistidas 
- Parental_Involvement: Nivel al que los padres han estado involucrados en los estudios de los hijos (Low, Medium, High)
- Access_to_Resources: Acceso a recursos educativos.  (Bajo, Medio, Alto)
- Extracurricular_Activities: Participación en actividades extraescolares (Si, no)
- Sleep_Hours: Media de horas de sueño por la noche
- Previous_Scores: Media de resultados obtenidos en examenes anteriores
- Motivation_Level: Nivel de motivación del estudiante (Bajo, Medio, Alto)
- Internet_Access: Disponibilidad de acceso a internet (Sí, No)
- Tutoring_Sessions: Número de sesiones de tutoría asistidas al mes
- Family_Income: Nivel de ingresos familiares (Bajo, Medio, Alto)
- Teacher_Quality: Calidad del profesor (Bajo, Medio, Alto)
- School_Type: Tipo de colegio (Público o privado)
- Peer_Influence: Influencia del grupo de iguales en el rendimiento académico (Positiva, Neutral, Negativa)
- Physical_Activity: Número medio de horas de actividad física por semana.
- Learning_Disabilities: Dificultades de aprendizaje (Sí, No)
- Parental_Education_Level: ivel educativo más alto alcanzado por los padres (Secundaria, Universidad, Posgrado)
- Distance_from_Home: Distancia del domicilio al centro educativo (Cerca, Media, Lejos)
- Gender: Género del estudiante (Masculino, Femenino)
- Exam_Score: Puntuación final del examen

## 4. Limpieza de datos
1. Analizo todas las columnas y me parecen útiles. Las dejo
2. Reviso que no hay celdas vacias. Solo encuentro en las columnas:
   Teacher_Quality
   Parental_Education_Level
   Distance_from_Home
   Estas filas no las elimino porque perdería bastantes datos. En su lugar pongo un "Unknown"
4. Reviso que las columnas con datos definidos (Yes/no, Low/Medium/High...) Están bien.
5. En datos numéricos miro que no haya datos sin sentido. Porcentajes mayor que 100
     En la columna Exam_Score hay un 101, por lo que elimino esa fila, ya que es solo una y sin el resultado del examen, esta fila no tiene importancia para el proyecto.
6. Y simplifico algunas columnas de valores numéricos para que sea más sencillo el análisis.
  Hours_Studied
  Attendance
  Sleep_Hours
  Previous_Scores
  Tutoring_Sessions
  Teacher_Quality
  Physical_Activity
  Exam_Score
    Dependiendo del valor bajo pongo Low, Medium o High

## 5. Análisis de datos
   He dividido las columnas en caracteristicas personales, familiares y académicas. Me he centrado en la nota final, no en      la de los parciales.
   Para cada una de las características, he creado una pestaña donde hay dos tablas dinámicas por característica:
      1. Nota media y número de alumnos por cada característica
      2. Dispersión de las notas por característica.
  
   Me quedo con las carácterísticas en las que haya más de 1,5 puntos entre el caso más desfavorable y el más favorable. Elijo solo 1,5 porque las notas son bastante homogeneas.
   Con esto hago un cuadro de mando para contrastar losp atrones observados en el análisis y un Dashboard

 ## 6. Dashboard  
   El dashboard presenta una visión general del rendimiento académico de los estudiantes, mostrando la distribución de las notas y nota media global. Incluye el análisis de los principales factores que influyen en los resultados. A través de gráficos comparativos, se observa cómo estas variables afectan a la nota media y a la distribución del rendimiento. 

  ## 7. Conclusiones
  La nota media es estable y con poca dispersión
  Las diferencias no son extremas pero hay factores como Acceso a recursos, Implicación parental, horas estudiadas y asistencia a clase (sobretodo las dos últimas) que separan mejor escenarios favorables vs desfavorables.
  El efecto se ve en el desplazamiento de la distribución, reducción de notas bajas y mayor concentración en notas medias-altas que en grandes saltos de media.
