# Diseño Generativo de Péptidos Antimicrobianos (AMP)

Pipeline de procesamiento de datos y modelado generativo condicional para el diseño de péptidos antimicrobianos con alta actividad biológica ($\text{MIC}$ bajo) y baja toxicidad hemolítica ($\text{HC}_{50}$ alto).

## Estructura del Proyecto

```text
proyecto-amp/
├── data_raw/                  # Datasets originales (Veltri, MIC experimental, sin etiquetar)
├── data_processed/            # Datasets limpios, unificados y particionados
│   ├── dataset_unificado.csv  # Dataset maestro (3,327 secuencias)
│   ├── train.csv              # Partición de entrenamiento (80%)
│   ├── val.csv                # Partición de validación (10%)
│   └── test.csv               # Partición de evaluación (10%)
├── wheels_hemopi2/            # Dependencias offline para predicción hemolítica (HemoPI2)
├── notebooks/
│   └── 01_exploracion_y_limpieza.ipynb
└── README.md
