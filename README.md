# COVID19 Radiology Pattern Recognition 
## Enunciado
Reconocedor automatico que a partir de una radiografia del torax de una persona sea capaz de diagnosticar si la persona tiene COVID19, Neuomonia o se encuentra sana. Para realizar este sistema de reconocimiento se cuenta con las imagenes radiograficas provenientes de la Italian Society of Medical and Interventional Radiology (SIRM) COVID-19 DATABASE. 


## Descripcion
Se cuenta con una base de datos de 6.300 patches en blanco y negro (escala de grises) de 64x64 pixeles, correspondientes a porciones de radiografias del torax pertenecientes a tres clases: 0-Normal, 1-Neumonia y 2-COVID19. La base de datos que emplearemos en la tarea se encuentra balanceada, es decir cada una de las clases cuenta con un tercio de las muestras. De la base de datos original, se ha extraido 210 radiografias por clase, y a cada radiografia se le extrajo 10 patches de 64x64 pixeles de las zonas mas oscuras del lado izquierdo de la radiografia.


Algunos ejemplos de radiografias y sus correspondientes 10 patches extraidos para cada una de las clases se muestran a continuacion:

<img src="https://github.com/domingomery/patrones/blob/master/tareas/Tarea_03/data/example.jpg" width="600">


La base de datos para esta tarea se encuentra disponible en los siguientes links:

* Training (1.680 patches por clase) [descargar](https://github.com/domingomery/patrones/blob/master/tareas/Tarea_03/data/train.zip)
* Testing (420 patches por clase) [descargar](https://github.com/domingomery/patrones/blob/master/tareas/Tarea_03/data/test.zip)

Los patches han sido guardados en archivos PNG con el siguiente nombre: Xmm_nnnn_ppp.png donde:

- 'X' es el caracter inicial de cada nombre de archivo
- mm: es 00, 01 o 02 segun la clase 0, 1, o 2 respectivamente
- nnnn: es el numero de la radiografia de la clase (0001, 0002,... 0168: para training, 0169, 0170, ... 0210 para testing)
- ppp: es el numero del patch extraido de la radiografia (001, 002, ... 010)  
