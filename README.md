# Titanic 🛳️
Trabajo Práctico para la materia **Base de Datos (TA044)**

## 📑Contenido

1. [Descripción](#descripción)
2. [Integrantes](#integrantes)
3. [Objetivos](#objetivos)
4. [Análisis Exploratorio](#análisis-exploratorio)
5. [Preprocesamiento](#preprocesamiento)
6. [Conclusiones](#conclusiones)

## 📄Descripción <a name="descripción"></a>

<div align="justify">
Este trabajo práctico consiste en desarrollar una aplicación que implemente el proceso de <b>ETL</b> (Extract, Transform, Load) sobre un conjunto de datos. El objetivo es limpiar, transformar y cargar los datos en una base de datos SQLite, garantizando que estén listos para ser utilizados en análisis posteriores. Para esto, se ha seleccionado el famoso dataset de Titanic, disponible en Kaggle.
</div>

**Dataset**: https://www.kaggle.com/datasets/akshaysehgal/titanic-data-for-data-preprocessing

## 👥Integrantes <a name="integrantes"></a>

| Nombre                    |
|---------------------------|
| Sebastián Brizuela        |
| Victoria Avalos           |
| Gonzalo Manuel Calderón   |
| Mateo Liberini            |
| Franco Agustín Rodriguez  |
| Urbano Sol Guadalupe      |

## 🎯Objetivos <a name="objetivos"></a>

- Implementar un flujo de trabajo **ETL** que incluya la extracción, transformación y carga de datos.
- Resolver problemas típicos de los datos, como valores nulos, duplicados y formatos inconsistentes.
- Garantizar que los datos estén listos para ser cargados y utilizados en una base de datos **SQLite**.

## 🔍Análisis Exploratorio <a name="análisis-exploratorio"></a>

<div align="justify">
El análisis comenzó con el dataset de Titanic, el cual contiene información relevante de los pasajeros, como edad, sexo, y si sobrevivieron o no. Se realizó un análisis exploratorio para obtener una vista general del dataset, observando la cantidad de filas, columnas y valores faltantes. Además, se generaron visualizaciones de la distribución de los datos y las relaciones entre las variables, como un boxplot para la distribución de la edad por sexo y un gráfico de barras para los valores nulos por columna.
</div>

## 🛠️Preprocesamiento <a name="preprocesamiento"></a>

Durante el preprocesamiento se tomaron varias decisiones clave:
- Eliminación de columnas redundantes como `male`, `class`, y `deck` (debido a gran cantidad de valores nulos).
- Imputación de valores nulos en la columna `age` basados en el promedio por sexo.
- Eliminación de filas duplicadas, manteniendo un registro por pasajero y añadiendo una columna extra con el número de duplicados.
- Normalización de los datos para asegurar consistencia en el formato.
- Finalmente, los datos se cargaron en una base de datos SQLite.

## 📝Conclusiones <a name="conclusiones"></a>

<div align="justify">
El proceso de ETL permitió identificar problemas en los datos, como valores faltantes, redundancias y duplicados, que fueron solucionados a través de técnicas de preprocesamiento. La base de datos resultante está lista para consultas SQL, lo que permite realizar análisis avanzados de manera eficiente. Este proyecto destacó la importancia de un correcto flujo de ETL en la preparación de datos para su análisis y visualización.
</div>

## 📄 Licencia  
Este proyecto está bajo la licencia MIT. Para más detalles, consulta el archivo [LICENSE](./LICENSE).
