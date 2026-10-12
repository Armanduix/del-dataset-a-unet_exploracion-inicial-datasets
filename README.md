# 🔎 Exploración inicial de un dataset de segmentación

Este repositorio contiene una práctica introductoria de **exploración de datasets de segmentación de imágenes**, desarrollada como parte del taller **«Del dataset a U-Net: segmentación de imágenes con Deep Learning»**.

---

## 🎯 Objetivo

Explorar la estructura y los componentes de un dataset de segmentación mediante herramientas de Python, identificando archivos, rutas, metadatos y anotaciones espaciales para comprender cómo se organiza la información que posteriormente utilizará un modelo de Deep Learning.

---

## 📁 Organización del proyecto

El notebook utiliza las siguientes ubicaciones dentro del repositorio:

```text
ejercicio_exploracion_dataset/
├── data/
│   └── raw/
│       ├── anotaciones.json
│       └── images/
│           ├── Chihuahua/
│           │   ├── Chihuahua_190.jpg
│           │   ├── Chihuahua_190.png
│           │   └── Chihuahua_190.xml
│           └── ...
└── notebooks/
    └── explorar_data.ipynb
```

Los archivos del minidataset se encuentran en `data/raw/`.

Cada categoría cuenta con su propio directorio, dentro del cual se almacenan conjuntamente las fotografías, máscaras y anotaciones individuales.

> [!NOTE]
> El minidataset contiene únicamente una pequeña selección de imágenes del Oxford-IIIT Pet Dataset original, reorganizada con fines didácticos. No representa el conjunto completo de datos.

---

## 💻 Requisitos

Para ejecutar la práctica se utilizan las siguientes bibliotecas:

| Biblioteca | Uso |
|---|---|
| `pathlib` | Construcción y exploración de rutas |
| `json` | Lectura de metadatos JSON |
| `xml.etree.ElementTree` | Lectura de anotaciones XML |
| `numpy` | Inspección de valores numéricos |
| `opencv-python` (`cv2`) | Lectura y procesamiento de imágenes |
| `matplotlib` | Visualización de imágenes y anotaciones |

También necesitarás un entorno compatible con Jupyter Notebooks.

---

---

## 📚 Dataset de referencia

**Oxford-IIIT Pet Dataset**

Parkhi, O. M., Vedaldi, A., Zisserman, A., & Jawahar, C. V. (2012). *Cats and Dogs*. IEEE Conference on Computer Vision and Pattern Recognition (CVPR).

[Consultar el dataset original →](https://www.robots.ox.ac.uk/~vgg/data/pets/)

El conjunto de imágenes utilizado en esta práctica es una selección reducida y reorganizada con fines didácticos. Su utilización debe respetar las condiciones de uso de las imágenes del dataset original.

---

## 🔗 Taller

Esta práctica forma parte del **Módulo 2 · Ingeniería del dataset** del taller:

[**Del dataset a U-Net: segmentación de imágenes con Deep Learning →**](https://github.com/bettypau-open-knowledge/del-dataset-a-unet)

**Bettypau Open Knowledge**

*Aprende · Experimenta · Construye · Comparte*