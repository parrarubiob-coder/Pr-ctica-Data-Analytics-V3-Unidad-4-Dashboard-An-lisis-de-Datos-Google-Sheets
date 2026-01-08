# Pr-ctica-Data-Analytics-V3-Unidad-4-Dashboard-An-lisis-de-Datos-Google-Sheets
Práctica de la unidad 4 Dashboard &amp; Análisis de Datos Google Sheets del curso Data &amp; Analytics V3
El objetivo de este proyecto es realizar un análisis exploratorio de datos y representarlo mediante un dashboard interactivo, utilizando Excel / Google Sheets.

## 1.Estructura del proyecto



## 2.Origen de los datos
El conjunto de datos utilizado en este proyecto corresponde a un dataset sobre factores que influyen en el rendimiento académico de los estudiantes.
Consta de 6.607 filas y 20 columnas

- Plataforma: Kaggle  
- Nombre del dataset: Student Performance Factors  
- Enlace: https://www.kaggle.com/datasets/lainguyn123/student-performance-factors

## 3. Limpieza de datos
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

   ## 4. Análisis de datos
   He dividido las columnas en caracteristicas personales, familiares y académicas. Me he centrado en la nota final, no en la de los parciales.
   Para cada una de las características, he creado una pestaña donde hay dos tablas dinámicas por característica:
      1. Nota media y número de alumnos por cada característica
      2. Dispersión de las notas por característica.
  
   Me quedo con las carácterísticas en las que haya más de 1,5 puntos entre el caso más desfavorable y el más favorable. Elijo solo 1,5 porque las notas son bastante homogeneas.
   Con esto hago un cuadro de mando para confirmar las suposiciones
   
