# Curso de object detection de platzi
Este es el curso de detección de objectos y segmentación de imagenes de Platzi.

## Primer notebook.
En el primer notebook, están los conceptos de ventana deslizante, y las metricas más usadas, entre ellas mAP y IOU.

### Arquitecturas.

<b>Backbone</b>: es una red pre-etrenada se usa para la clasificación, solo se saca las caracteristicas de las imagenes y a partir de ahí se clasifican y se hayan los bounding box

las arquitecturas se dividen en dos:
   * <b>Multietapa</b>: Dada una imagen se generan varias regiones donde pueden estar los objectos. Luego cada región es pasada por la red para clasificar los objectos. Los algorimos más utilizados para buscar la regiones son selective search y (RPN).
     * Las redes que lo implementa son la familia de las R-CNN
   * <b>Una etapa:</b> Dada una imagen, en un solo pasó (Son más rápidas):
     * Las redes que la implementan son, SDD, YOLO, RetinaNet,EfficientDet
   * <b>Basadas en Transformers</b>: Usan los transformers para hacer la detección. Todavía está en investigación.
     * La más común es DERT.

## Segundo notebook.
El sengundo es un noteboo de un tutorial para hacerle fine-tuning a un modelo de detección, esto se hace por medio de una librería que se llama  tensorflow-zoo

## notebook segmentación
Es un tutorial para entranar un modelo de segementación, se montó la U-net con keras.