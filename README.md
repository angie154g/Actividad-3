#  Actividad 3 – Transformación y Unificación de Datos

Este proyecto tiene como objetivo transformar, limpiar y unificar información sobre ferias del libro en México, a partir de tres fuentes contenidas en un archivo Excel. El resultado es un dataset consolidado y listo para análisis o visualización posterior.

---

##  Objetivos

- Usar funciones de transformación como `pivot_longer`, `separate`, `mutate`, `case_when` y `joins` para unificar datasets.
- Crear variables adicionales útiles, como la región geográfica.
- Documentar el flujo completo de transformación con `dplyr` y `%>%`.
- Guardar el script en `scripts/transform.R` y el dataset final en `data/processed/final_dataset.csv`.

---

##  Estructura del Proyecto

```
proyecto/
├── data/
│   ├── raw/
│   │   └── feria_libro_directorio.xlsx
│   └── processed/
│       └── final_dataset.csv
├── scripts/
│   └── transform.R
├── actividad3_transformacion.Rmd
└── README.md
```

---

##  Requisitos

Este proyecto usa R y los siguientes paquetes:

```r
install.packages(c("dplyr", "readr", "readxl", "tidyr", "stringr", "here"))
```

Asegúrate de instalar estos paquetes **desde la consola de R**, no dentro del `.Rmd`.

---

##  Cómo ejecutar

###  Opción 1: Ejecutar el script directamente

Abre tu consola de R o RStudio y corre:

```r
source("scripts/transform.R")
```

Esto leerá, limpiará y exportará el dataset final a `data/processed/final_dataset.csv`.

###  Opción 2: Knit el archivo `.Rmd`

Compila el archivo `actividad3_transformacion.Rmd` usando el botón **Knit** para obtener un reporte en HTML con todo el análisis y el resultado.

---

##  Resultado Final

El archivo final `final_dataset.csv` contiene:

- ID y nombre de la feria
- Información de contacto
- Ubicación y coordenadas geográficas
- Nombre de la entidad
- Una columna nueva: `region`, basada en la entidad federativa

---

## 
Angélica Benítez
 Agosto 2025
