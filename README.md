# Pr-ctica-Data-Analytics-V3-Unidad-4-Dashboard-An-lisis-de-Datos-Google-Sheets
Práctica de la unidad 4 Dashboard &amp; Análisis de Datos Google Sheets del curso Data &amp; Analytics V3

## Origen de los datos

El conjunto de datos utilizado en este proyecto corresponde a un dataset sobre factores que influyen en el rendimiento académico de los estudiantes.

- Plataforma: Kaggle  
- Nombre del dataset: Student Performance Factors  
- Enlace: https://www.kaggle.com/datasets/lainguyn123/student-performance-factors

## 1. Limpieza de datos
1. Analizo todas las columnas y me parecen útiles. Las dejo
2. Reviso que no hay celdas vacias. Solo encuentro en las columnas:
   Teacher_Quality
   Parental_Education_Level
   Distance_from_Home
   Estas filas no las elimino porque perdería bastantes datos. En su lugar pongo un "Unknown"
4. Reviso que las columnas con datos definidos (Yes/no, Low/Medium/High...) Están bien.
5. En datos numéricos miro que no haya datos sin sentido. Porcentajes mayor que 100
     En la columna Exam_Score hay un 101, por lo que elimino esa fila
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
