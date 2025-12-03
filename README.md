[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=Silva22211767/ProyectoFinal)

# ProyectoFinal
Modelado de Membrana Neuronal: Hiperexcitabilidad Epiléptica

## Información de los estudiantes
María Fernanda Almazán Pacheco \[22211744]; l22211744@tectijuana.edu.mx

María Fernanda Antúnez Rubio \[22211745]; l22211745@tectijuana.edu.mx

Carlos Azael Ramírez Rodríguez \[22212267]; l22212267@tectijuana.edu.mx

Karla Emilia Silva Perez \[22211767]; l22211767@tectijuana.edu.mx

Modelado de Sistemas Fisiológicos

Ingeniería Biomédica

## Docente
Dr. Paul Antonio Valle Trujillo; paul.valle@tectijuana.edu.mx

Departamento de Ingeniería Eléctrica y Electrónica, Tecnológico Nacional de México/IT Tijuana, Blvd. Alberto Limón Padilla s/n, Tijuana, C.P. 22454, B.C., México.

## Descripción de la asignatura

El modelizado de sistemas fisiológicos es una herramienta importante en Ingeniería Biomédica, permite comprender el funcionamiento del cuerpo humano, así como diseñar y evaluar terapias y dispositivos médicos; se define como el proceso de formular modelos matemáticos o computacionales que representan el comportamiento y la interacción de los sistemas biológicos y fisiológicos. Esta asignatura pretende aportar al perfil del Ingeniero Biomédico la capacidad de realizar investigación científica en el área de Biología de Sistemas con la finalidad de dirigir y participar en equipos de trabajo interdisciplinarios en contextos nacionales e internacionales, así como de proporcionar soluciones informáticas para resolver problemas en el campo de la Ingeniería Biomédica con ética profesional; lo anterior al proporcionar al estudiante bases sólidas para modelizar sistemas y diseñar controladores para la solución de problemas en las áreas de atención médica y del sector industrial médico. La construcción de analogías entre circuitos eléctricos y sistemas fisiológicos para la formulación de modelos matemáticos y el diseño de controladores mediante la experimentación in silico brindan herramientas de gran aplicación en el quehacer profesional del Ingeniero Biomédico.

La asignatura de Modelado de Sistemas Fisiológicos forma parte del plan de estudios de la carrera en Ingeniería Biomédica con la siguiente competencia general del curso: Utiliza las propiedades de los circuitos RLC para describir la dinámica de sistemas fisiológicos, obtener modelos matemáticos y aplicar el control clásico, esto con el objetivo de integrar los principios de la Ingeniería de Control, la Electrónica Analógica y las Ciencias de la Computación con la Anatomía y Fisiología del cuerpo humano para proporcionar descripciones cuantitativas y cualitativas de sistemas fisiológicos complejos con el objetivo de modelizar, analizar, controlar, ilustrar y predecir su dinámica tanto en el corto como en el largo plazo.

## Objetivos
1. Calcular la función de transferencia.
2. Determinar el modelo de ecuaciones integro-diferenciales.
3. Calcular el error en estado estacionario y la estabilidad en lazo abierto.
4. Emular y simular la respuesta del circuito en Simulink/Simscape.
5. Sintonizar las ganancias de un controlador PID para eliminar el error entre la entrada y la salida del sistema.
   
## Descripción detallada del sistema

La membrana de una neurona cortical puede representarse, desde el punto de vista eléctrico, como un sistema lineal equivalente que captura su capacidad para almacenar y disipar carga, así como la presencia de corrientes iónicas lentas responsables de la modulación de la excitabilidad. En este modelo, la membrana se aproxima mediante un circuito del tipo R–L–C, donde:

-C corresponde a la capacitancia de la membrana, que refleja la capacidad del bilípido para acumular carga y determinar la velocidad a la que el voltaje de membrana responde a una corriente entrante.

-R representa la conductancia pasiva o de fuga, que modela el flujo de iones a través de canales de fuga abiertos en reposo. Esta resistencia actúa como una fuerza de amortiguamiento que tiende a llevar el potencial de membrana hacia el potencial de reposo.

-L se utiliza para aproximar el efecto de corrientes iónicas lentas (por ejemplo, corrientes de calcio o sodio persistente) que introducen una componente inercial en la respuesta eléctrica. Esta inductancia efectiva permite representar el retardo fisiológico con el que estos canales se activan o desactivan ante cambios en el voltaje.

La epilepsia se caracteriza por un estado de hiperexcitabilidad neuronal, en el cual pequeñas entradas sinápticas son capaces de generar respuestas de gran amplitud o repetitivas. Esta condición puede modelarse como una alteración de los parámetros del circuito R–L–C.

-Condición control (neurona sana): Los valores de R, L y C se encuentran dentro de rangos fisiológicos que aseguran un equilibrio adecuado entre excitación y amortiguamiento. Bajo un estímulo dado, el potencial de membrana responde con una dinámica amortiguada, generando una despolarización transitoria que retorna al reposo sin generar oscilaciones sostenidas.

-Condición caso (neurona hiperexcitable / epiléptica):

La hiperexcitabilidad puede representarse mediante:

  -Disminución de R, lo que equivale a un incremento en la conductancia excitatoria o una reducción del efecto estabilizador de los canales de fuga.

  -Reducción de C, lo que hace que la membrana cambie más rápidamente de voltaje ante una corriente entrante.

  -Disminución del amortiguamiento asociado a L, lo cual permite que las corrientes lentas contribuyan a respuestas de mayor amplitud o incluso a oscilaciones subamortiguadas.

En conjunto, estas modificaciones desplazan al sistema hacia un régimen en el que una misma entrada sináptica genera una respuesta mucho mayor o incluso autoamplificada, reproduciendo el comportamiento de una neurona hiperexcitable como la que se encuentra en un foco epiléptico.

Palabras clave: Circuito RLC; Controlador PID; Sistema nervioso; Modelo matemático; Neurona.

## Lista de archivos incluidos en el repositorio
1. Cuaderno computacional de MATLAB [.mlx].
2. Modelo de Simulink [.slx].
3. Imagen con los parámetros del controlador.
4. Imágenes de las simulaciones [.pdf y .png].
5. Evidencia del análisis matemático: función de transferencia, modelo de ecuaciones integro-diferenciales, error en estado estacionario y estabilidad en lazo abierto.

## Referencias
[1] P. A. Valle, Syllabus para Modelado de Sistemas Fisiológicos, Tecnológico Nacional de México / Instituto Tecnológico de Tijuana, Tijuana, B.C., México, 2025. Permalink: https://biomath.xyz/course/

[2] M. C. Khoo, Physiological Control Systems Analysis Simulation, and Estimation, 2nd ed. Piscataway, New Jersey, USA: IEEE Press, 2018, Section 4, Page 93.

[3] N. S. Nise, Control Systems Engineering, 8th ed. Hoboken, New Jersey, USA: John Wiley & Sons, 2020.

[4] T. Kind, T. J. Faes, J. W. Lankhaar, A. Vonk-Noordegraaf 
