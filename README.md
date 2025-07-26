# PURIFICADOR DE AIRE EN ESPACIOS CERRADOS 


## Integrantes:

-José Luis Ramirez Isaza.

-Camilo Andres Marquez Blanco

-Cristian David Ramirez Plazas


## Descripción/Introducción

Este proyecto fue desarrollado en el marco del curso de Taller de Electrónica. Su propósito es diseñar un sistema de ventilación automática para espacios cerrados como minas, cuartos técnicos o túneles, donde se pueden acumular gases nocivos o humo, poniendo en riesgo la salud humana.

La solución consiste en un sistema embebido basado en ESP32, capaz de detectar concentraciones peligrosas de gases mediante sensores como el MQ-2 o MQ-135, y accionar extractores de aire automáticamente. Para la implementación se diseñó y fabricó una PCB que integra todos los componentes requeridos, buscando robustez, bajo consumo energético y facilidad de mantenimiento.

Este proyecto busca no solo resolver un problema real, sino también aplicar conocimientos técnicos en electrónica, diseño de circuitos, programación y manufactura digital.




## Palabras clave

ESP32, sensores de gas, ventilación automática, sistema embebido, PCB, MQ-2, humo, seguridad industrial, electrónica digital, automatización.

## Poster 
-Poster del proyecto:
<img width="1414" height="2000" alt="poster" src="https://github.com/user-attachments/assets/1c5506ea-f13a-4c18-8f37-385a26916b15" />


## Banner
-Banner:

## Video del proyecto
-Video del proyecto
[sistema de ventilacion](https://choosealicense.com/licenses/mit/)



# CONTEXTO
## Problemática
En diversos entornos industriales y subterráneos, como minas, bodegas cerradas o cuartos técnicos, existe un riesgo constante de acumulación de gases tóxicos o inflamables, así como humo en caso de incendios o fallas eléctricas. La exposición prolongada a estas condiciones puede provocar intoxicaciones, incendios o explosiones.

En muchos de estos lugares, no se cuenta con sistemas de monitoreo y ventilación automáticos que permitan detectar y evacuar estos gases de manera eficiente. Las soluciones comerciales existentes suelen ser costosas o difíciles de adaptar a espacios pequeños o de bajo presupuesto.

Esta problemática hace necesario el desarrollo de un sistema autónomo, económico, eficiente y fácil de implementar, que permita detectar condiciones peligrosas y activar mecanismos de ventilación sin intervención humana inmediata.
## Objetivos
Objetivo general:
Desarrollar un sistema automático de ventilación para espacios cerrados que detecte la presencia de humo o gases nocivos y active un sistema extractor de forma inmediata, utilizando una ESP32 y una PCB diseñada a medida.

Objetivos específicos:
Diseñar una PCB funcional para integrar sensores de gas, actuadores y microcontrolador.

-Implementar el código embebido para el control automático del sistema.

-Fabricar una carcasa o encapsulado funcional para alojar los componentes.

-Evaluar el sistema en un entorno de prueba simulando condiciones reales.

-Documentar el proceso de diseño, implementación, pruebas y resultados.
## Alcance de proyecto
 Incluye:

-Diseño y fabricación de una PCB funcional

-Programación del sistema embebido usando ESP32

-Integración de sensores de gas (como MQ-2)

-Activación automática de ventilador al detectar gases

-Ensamblaje del prototipo con carcasa física

-Pruebas en laboratorio o entornos controlados

No incluye:

-Implementación en campo real (mina o espacio industrial real)

-Monitoreo remoto vía Wi-Fi o app (se puede proponer como mejora futura)

-Alimentación con baterías recargables o sistema autónomo de energía
## Ruta / Roadmap del Proyecto
<img width="615" height="123" alt="roadmap" src="https://github.com/user-attachments/assets/c643b672-fba3-4c89-b5c8-17315db5e03c" />

## DISEÑO DE LA SOLUCION
## Diagrama de caja negra
![diagrama de caja negra](https://github.com/user-attachments/assets/a271bb0e-c49a-4000-8f97-3bd62392d777)

## Diagramas tecnológicos
<img width="739" height="338" alt="diagrama tegnologico" src="https://github.com/user-attachments/assets/88c82709-8c34-4726-995c-78cef43e4bac" />

## Diagrama de flujo general del proyecto
![diagrama de flujo](https://github.com/user-attachments/assets/7a142cd2-7b1b-46ce-99fe-ad4b078d8f44)

## Impacto ambiental y acciones propuestas de mitigación
Impacto:
Uso de componentes electrónicos que, si no se disponen correctamente, pueden contaminar suelos y aguas.

Consumo de energía eléctrica, especialmente en la etapa de pruebas.

Mitigación:
Reutilización de componentes electrónicos y reciclaje de residuos electrónicos.

Reducción del uso de prototipos físicos mediante simulaciones previas (en KiCad o Proteus).

Uso de impresión 3D con materiales reciclables como PETG o PLA.

Implementación futura de alimentación mediante energía solar para hacerlo autónomo.

# DISEÑO E IMPLEMENTACION 
## Diseño del Case (Corte 3D)
##  Imágenes del diseño
## Evidencias de implementación física
## Evidencias de implementación física

# DISEÑO E IMPLMENTACION ELECTRONICA
## Simulaciones (opcional)
Se realizaron simulaciones básicas del circuito con herramientas como Tinkercad o Proteus, para validar el funcionamiento del sensor MQ-2, el control del ventilador mediante transistor y la lógica de activación. Estas simulaciones ayudaron a verificar que las conexiones lógicas eran correctas antes de fabricar la PCB.

##  Bocetos y esquemas preliminares
Durante la etapa de diseño se elaboraron esquemas a mano en papel o tablero, para discutir en equipo la distribución de pines, los componentes necesarios y la topología del circuito.
![boceto circuito](https://github.com/user-attachments/assets/a09225d1-c073-4878-9eee-6c35fdb65a63)


## Diseño de PCB en KiCad

Esquemático del circuito
El esquemático fue desarrollado en KiCad, incluyendo los siguientes elementos:

Sensor MQ-2

ESP32

Transistor/MOSFET para control del ventilador

Buzzer y LEDs

Conectores y terminales

# Layout (ruteo de pistas)
---------


#  Render 3D de la PCB
Se generó una vista 3D del diseño final para verificar disposición de componentes y facilitar el diseño del encapsulado.
# Fabricación de la PCB
Foto de la PCB fabricada (vacía):


Foto con componentes soldados:


Foto con sensores y actuadores conectados:

# DISEÑO E IMPLEMENTACION DEL SOFTWARE
## Diagramas de flujo de tareas del sistema
![diagrama de software](https://github.com/user-attachments/assets/a61533ac-5d81-4139-b123-7cea5ed9cb5b)

## Código y pruebas unitarias
Se desarrollaron scripts de prueba para cada componente:

Lectura del sensor MQ-2

Activación de ventilador vía transistor

El código fue implementado en Jhonny IDE, y estructurado por módulos (setup, lectura, lógica de decisión, salidas).
##  Interacción con interfaces externas
Se programaron posibles pines para integración con una app móvil o una interfaz serial (monitor de Arduino).

Opcionalmente se dejó preparado el código para incluir Wi-Fi (ESP32).

# EVIDENCIAS
## Proceso de integración y ensamble
Montaje físico del sistema:

Errores comunes detectados:

Inversión de conexiones en el sensor

Baja sensibilidad del MQ-2 sin precalentamiento

Error de ruteo en la primera versión de la PCB

Aciertos importantes:

Uso de terminales para fácil conexión

Tamaño compacto del diseño

Buen aislamiento del encapsulado

# CONCLUSIONES
El proyecto permitió avanzar significativamente en el diseño e integración de un sistema de ventilación automática para espacios cerrados, aplicando conocimientos en electrónica, programación embebida y diseño de PCB. Se logró desarrollar un prototipo funcional a nivel de hardware y software, con pruebas exitosas de componentes individuales.

Sin embargo, el proyecto no se terminó de concretar completamente debido a diversos fallos durante la etapa de integración final, como problemas de ruteo en la PCB, errores en las conexiones y sensibilidad inconsistente del sensor de gas. Estos inconvenientes impidieron alcanzar una validación completa del sistema en condiciones reales.

A pesar de ello, el proceso dejó importantes aprendizajes sobre el trabajo iterativo, la importancia de las pruebas tempranas, el manejo de fallos y la necesidad de una buena planificación en cada etapa de desarrollo.

## Recomendaciones para futuros trabajos
Para futuros desarrollos similares, se recomienda realizar pruebas exhaustivas de cada módulo de manera individual antes de proceder a la integración final, especialmente cuando se diseñan PCBs personalizadas. Además, es fundamental verificar cuidadosamente el ruteo de pistas, la orientación de componentes y las conexiones críticas del circuito en la etapa de diseño.

También se sugiere dejar tiempo suficiente para iterar al menos una vez sobre la PCB, ya que es común encontrar errores en la primera versión. Finalmente, explorar sensores más estables o precalibrados, así como módulos de comunicación para monitoreo remoto, podría mejorar la confiabilidad y funcionalidad del sistema.





