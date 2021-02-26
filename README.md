# DS-ONLINE-57

## Sprint3

<br> Mentor: Federico Moreno <br/>
<br> Email: federicomoreno613@gmail.com <br/>



### Estructura del repositorio

La estructura del repositorio simplemente es el orden de las carpetas de un proyecto. Cada team puede tener su convención y su orden. Cuestión que luego puede devenir en problemas de **reproducibilidad** del proyecto respecto a otros equipos.

```
proyecto_ejemplo/
├── data/ 
│   └── original            Data inmutable, en lo posible raw de una fuente de datos
|   └── procesada           Data preprocesada, ejemplo con nuevas columnas transformadas o limpia
│ 
├── laboratory/             notebooks en una instancia de laboratorio
│   └── EDA                 Exploración de la data
│   └── preprocessing       Preprocesamiento de la data, posiblemente para creación de features
│   └── model_training      Implementaciones de algoritmos
│   └── evaluation          Testeo y evaluación
|
├── figures/                Imagenes guardadas de plots o resultados
├── output/                 outputs, pesos de modelos, prediccion o hiperparámetros óptimos 
├── source/                 modulos creados por nosotros
│   └── __init__.py      Make the folder a package.
    └── process.py       Example module.
├── environment.yml      Virtual environment definition.
├── README.md            README with info of the project.
└── requeriments.txt     Install requeriments.
```

Hay dos grandes tipos de repositorios para nuestra profesión, los que están en modo laboratorio (cómo el nuestro) y los que están en modo producción en los cuales desarrollan un "pipeline" 

Los equipos tienden a comenzar con un flujo de trabajo manual, donde no existe una infraestructura real. La recopilación de datos, la limpieza de datos, el entrenamiento de modelos y la evaluación probablemente se escriban en un solo cuaderno. El cuaderno se ejecuta localmente para producir un modelo, que se entrega a un ingeniero encargado de convertirlo en un punto final de API. Esencialmente, en este flujo de trabajo, el modelo es el producto.

Características de una canalización de ML manual:

El modelo es el producto
Proceso manual o guiado por script
Una desconexión entre el científico de datos y el ingeniero
Ciclo de iteración lento
Sin pruebas automatizadas ni supervisión del rendimiento
Sin control de versiones


Características de una canalización de ML automatizada:

La tubería es el producto
Proceso completamente automatizado
Cooperación entre el científico de datos y el ingeniero
Ciclo de iteración rápido
Supervisión automatizada de pruebas y rendimiento
Controlado por versión
El enfoque de canalización permite escalar el aprendizaje automático
La transición de un ciclo manual a una canalización automatizada puede tener muchas iteraciones en el medio, según la escala de sus esfuerzos de aprendizaje automático y la composición de su equipo. En última instancia, el propósito de una canalización es permitirle aumentar el ciclo de iteración con la confianza adicional que brinda la codificación del proceso y escalar cuántos modelos puede mantener de manera realista en producción.

Machine Learning pipelines with Spark ML


https://medium.com/@Sushil_Kumar/machine-learning-pipelines-with-spark-ml-94cd9b4c973d

