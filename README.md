# PROY-2026-GRUPO7

Repositorio del grupo X para el proyecto del ramo *Proyecto Inicial (IWG400)* – 2026.

## 👥 Integrantes del grupo

| Nombre y Apellido | Usuario GitHub | Correo USM               | Rol USM      |
| ----------------- | -------------- | ------------------------ | ------------ |
| Benjamín Cerda | @bcerdafilippi     | bcerdaf@usm.cl | 2026300420 |
| Amira Lizana  | @Tiar-e     | alizana@usm.cl | 2026300056|
| Santiago Silva | @Santouc      | ssilvap@usm.cl | 2026300099 |

"Es un software capaz de aprender cualquier lenguaje de señas basado en el reconocimiento de la mano en 21 puntos a través de una cámara. Nuestra motivación al realizar este proyecto es facilitar la comunicación entre las personas sordomudas y el resto de la sociedad."

---

## 🎯 Objetivos

- Objetivo general:
  - Crear un software, el cual sea capaz de aprender cualquier lenguaje de señas en base a un entrenamiento del software mediante fotogramas y la detección de la forma de la mano
- Objetivos específicos:
   La capacidad del software de poder detectar sin mayores problemas la forma y posición de la mano.
---

## 🧩 Alcance del proyecto

Es un modelo capaz de aprender un lenguaje de señas, tanto estáticas como dinámicas.
Lo que queda fuera del alcance es la integración al sistema Arduino Uno Q, debido a limitaciones de tiempo y hardware.

## 🛠️ Tecnologías y herramientas utilizadas

- Lenguaje(s) de programación:
  - Python, Json

---

## 🗂️ Estructura del repositorio

```
/Mimo
│
├── api/                        # API REST para servir el modelo
│   ├── Dockerfile              # Imagen Docker de la API
│   ├── README.md               # Documentación de la API
│   ├── client_examples.py      # Ejemplos de cliente para consumir la API
│   ├── docker-compose.yml      # Orquestación de contenedores
│   ├── main.py                 # Punto de entrada del servidor API
│   └── requirements.txt        # Dependencias de la API
│
├── core/                       # Lógica central de visión y datos
│   ├── dataset_utils.py        # Utilidades para manejo de datasets
│   ├── hand_detector.py        # Detección de manos (MediaPipe)
│   ├── image_processor.py      # Procesamiento de imágenes
│   └── preprocessing.py        # Preprocesamiento de landmarks
│
├── ml/                         # Machine Learning (entrenamiento e inferencia)
│   ├── __init__.py             # Inicializador del paquete
│   ├── clasificador.py         # Clasificador de señas estáticas
│   ├── data_capture.py         # Captura de datos de entrenamiento
│   ├── data_processor.py       # Procesamiento de datos
│   ├── deployment_manager.py   # Gestión de despliegue de modelos
│   ├── dynamic_classifier.py   # Clasificador de señas dinámicas
│   ├── model_evaluator.py      # Evaluación de modelos
│   ├── realtime_optimizer.py   # Optimización en tiempo real
│   ├── train.py                # Entrenamiento del modelo estático
│   └── train_dynamic.py        # Entrenamiento del modelo dinámico
│
├── data/                       # Datos y modelos entrenados
│   ├── datasets/               # Datasets de entrenamiento
│   │   ├── dataset_dynamic.json    # Dataset de señas dinámicas
│   │   └── dataset_static.json     # Dataset de señas estáticas
│   └── models/                 # Modelos y etiquetas
│       ├── hand_landmarker.task    # Modelo de landmarks de MediaPipe
│       ├── labels.json             # Etiquetas estáticas
│       ├── labels_dynamic.json     # Etiquetas dinámicas
│       ├── model.h5                # Modelo estático entrenado
│       └── model_dynamic.h5        # Modelo dinámico entrenado
│
├── utils/                      # Utilidades generales
│   ├── __init__.py             # Inicializador del paquete
│   ├── config.py               # Configuración del proyecto
│   └── logger.py               # Sistema de logging
│
├── docs/                       # Documentación general y reportes
│   ├── anexo_tecnico.md        # Anexo técnico
│   ├── conceptos.md            # Conceptos teóricos
│   └── manual_uso.md           # Manual de uso
│
├── logs/                       # Archivos de registro (logs)
├── models/                     # Carpeta de modelos (auxiliar)
├── temp/                       # Archivos temporales
│
├── main.py                     # Aplicación principal (reconocimiento en vivo)
├── teaching.py                 # Herramienta de captura y enseñanza de señas
├── dataset_static.json         # Dataset de señas estáticas (raíz)
├── requirements.txt            # Dependencias del proyecto
├── .gitignore                  # Archivos ignorados por Git
└── README.md                   # Este archivo
```

---

## 🚀 Instrucciones de Instalacion y Uso


1. **Clonar el repositorio:** `git clone ...`
2. **Dependencias:** Listar qué librerías necesitan (ej: `pip install -r requirements.txt` o librerías de Arduino).
3. **Ejecución:** Cómo se corre el código principal.

---



## 📅 Cronograma de trabajo

[Carta Gantt](https://google.com)
https://usmcl-my.sharepoint.com/:x:/g/personal/ssilvap_usm_cl/IQAZlQx4230hTY1oSzXnhvYKAcZ4onZFIGCQQ6yur6llBPo?e=g9aMB9
---

## 📚 Bibliografía

[Enlace](https://google.com)

---

## 📌 Notas adicionales

> *Espacio para dejar cualquier comentario útil, como pendientes, acuerdos del grupo, consideraciones especiales, etc.*
