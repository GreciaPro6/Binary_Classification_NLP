# Proyecto de Análisis de Sentimiento en IMDB

Este proyecto entrena una red neuronal para analizar sentimientos en reseñas de películas utilizando el conjunto de datos IMDB. Se usa `Keras` con `TensorFlow` como backend para la construcción y entrenamiento del modelo.

## Estructura del Proyecto

```
/
├── requirements.txt  # Dependencias necesarias
├── src/              # Carpeta con código fuente
├── .gitignore        # Archivos a ignorar en Git
├── README.md         # Documentación del proyecto
├── main.py           # Script principal que ejecuta el modelo
```

## Requisitos

Antes de ejecutar el proyecto, asegúrese de instalar las dependencias necesarias con el siguiente comando:

```bash
pip install -r requirements.txt
```

## Uso

Para entrenar y evaluar el modelo, ejecute el siguiente comando en la terminal:

```bash
python main.py
```

Esto cargará el conjunto de datos de IMDB, entrenará una red neuronal y mostrará las gráficas de pérdida y precisión durante el entrenamiento.

## Descripción del Modelo

El modelo de red neuronal consta de:

- Tres capas densas:
  - Capa densa con 16 neuronas y activación ReLU (entrada de 10,000 dimensiones)
  - Capa densa con 16 neuronas y activación ReLU
  - Capa de salida con activación sigmoide para clasificación binaria

Se entrena con `rmsprop` como optimizador y `binary_crossentropy` como función de pérdida.

## Visualización de Resultados

El entrenamiento genera gráficas de:
- Pérdida en entrenamiento y validación
- Precisión en entrenamiento y validación

Estas ayudan a evaluar el rendimiento del modelo.
