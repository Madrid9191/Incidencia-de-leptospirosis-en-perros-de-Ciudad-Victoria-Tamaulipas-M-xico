# Incidencia de leptospirosis en perros de Ciudad Victoria, Tamaulipas, Mexico

## Introduction

En este estudio de caso, realizaré muchas tareas del mundo real de un analista de datos junior. Trabajaré con datos obtenidos de distintas veterinarias de Ciudad Victoria que representan a perros con dianostico de leptospirosis. Para responder las preguntas clave, seguiré los pasos del proceso de análisis de datos: preguntar, preparar, procesar, analizar, compartir y actuar.

### Quick links:

## Background

La leptospirosis es una enfermedad zoonótica que afecta tanto a la salud humana como a la sanidad animal, con graves repercusiones económicas y sociales (Rodríguez, 2018). Es causada por bacterias del género Leptospira spp., y es de distribución mundial tanto en áreas urbanas como rurales (Ospina-Pinto & Rodríguez, 2015; Rodríguez, 2018). La transmisión hacia otros animales y personas ocurre por el contacto con el agua, suelo o vegetación contaminada con orina de animales que son hospederos de Leptospira sp. (Rodríguez, 2018). En los caninos el contacto directo es la vía más importante de transmisión, bien sea por la aspersión de gotas de orina cuando ellos marcan su territorio o al lamer los genitales de sus congéneres (Murhekar et al., 1998; Faine et al., 1999; Luna et al., 2008). La leptospirosis en los caninos varía de factores como la edad, de la respuesta inmune y de la serovariedad implicada (Faine et al., 1999). Los caninos alojan el agente patógeno en los riñones, pudiéndose excretar por largos períodos, convirtiéndolos en un riesgo de infección importante para los humanos (McDonough, 2001; Blazius et al., 2005; Moore et al., 2006; Andre-Fontaine, 2006).

## Ask

### Business task

Determinar la prevalencia de leptospira spp en perros domésticos de Ciudad Victoria, durante un período de un año, con el fin de obtener datos epidemiológicos relevantes que contribuyan a la prevención y control de la leptospirosis en esta población canina y promuevan la salud pública en la comunidad.

### Analysis Questions

- ¿Cuál es la colonia con mas casos de Leptospira spp en perros domésticos de Ciudad Victoria?

- ¿Cual es el rango de edad con mas casos de Leptospira spp?

- ¿Hay mas hembras o machos infectados con Leptospira spp?

- ¿Los perros vacunados son mas propensos a infectarse de Leptospira spp?

- ¿Durante cual mes y temporada hay mas casos de Lepstosipira spp?

## Prepare

### Data source

Identificare y analisare tendencia en los datos obtenidos de la veterinaria sobre perros con diagnostico presuntivo de leptospirosis obtenidos de septiembre del 2020 a junio de 2021 y ademas se calculara la prevalencia y se realizara una analisis de Chi2 para idependencia de muestras. Los datos originales pueden ser descargados en Leptospira

### Data Organization

Hay un unico archivo de excel con la inforacion obtenida durante septiembre del 2020 a junio del 2021. El archivo incluye 10 columnas con los siguientes nombres NOMBRE, SEXO, EDAD, EDAD, RAZA, VACUNACION,  FECHA, ZONA, MAT, ELISA y PCR.

## Data exploration
El archivo fue cargado como una tabla. Explorar los datos me permitio darme cuenta que la columna EDAD deberia esatr en formato numerico pero esta en formato caracter. Tambien la columna FECHA deberia estar en formato fecha pero esta en formato caracter. Ademas se necesita crear dos nuevas columnas una con el año en que se tomo la muestra y otra con el mes en que se tomo la muestra. Asi mismo las columnas MAT, ELISA y PCR representan las distintas pruebas que se realizaron para saber si los perros estabn enfermos de leptospirosis, asi que se necesita combinar los resultados de las tres columnas y tambien solo hay que remplazar uno de los dos posibles resultados "neg" por "negativo".

## Data Cleaning

- El formato de la columna EDAD fue cambiado de caracter a numeric
- EL formato de la columna FECHA fue cambiado de caracter a fecha
- Tres columnas fueron creadas AÑO, MES y RESULTADO 







