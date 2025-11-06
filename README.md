[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=l22212265/Practica6MSF)

# Práctica: Regeneración de globulos rojos

## Información de la estudiante

Yoseline Lizeth Puentes Hernandez \[22212265]; l22212265@tectijuana.edu.mx

Modelado de Sistemas Fisiológicos

Ingeniería Biomédica

## Docente

Dr. Paul Antonio Valle Trujillo; paul.valle@tectijuana.edu.mx

Departamento de Ingeniería Eléctrica y Electrónica, Tecnológico Nacional de México/IT Tijuana, Blvd. Alberto Limón Padilla s/n, Tijuana, C.P. 22454, B.C., México.

## Descripción de la asignatura

El modelizado de sistemas fisiológicos es una herramienta importante en Ingeniería Biomédica, permite comprender el funcionamiento del cuerpo humano, así como diseñar y evaluar terapias y dispositivos médicos; se define como el proceso de formular modelos matemáticos o computacionales que representan el comportamiento y la interacción de los sistemas biológicos y fisiológicos. Esta asignatura pretende aportar al perfil del Ingeniero Biomédico la capacidad de realizar investigación científica en el área de Biología de Sistemas con la finalidad de dirigir y participar en equipos de trabajo interdisciplinarios en contextos nacionales e internacionales, así como de proporcionar soluciones informáticas para resolver problemas en el campo de la Ingeniería Biomédica con ética profesional; lo anterior al proporcionar al estudiante bases sólidas para modelizar sistemas y diseñar controladores para la solución de problemas en las áreas de atención médica y del sector industrial médico. La construcción de analogías entre circuitos eléctricos y sistemas fisiológicos para la formulación de modelos matemáticos y el diseño de controladores mediante la experimentación in silico brindan herramientas de gran aplicación en el quehacer profesional del Ingeniero Biomédico.

La asignatura de Modelado de Sistemas Fisiológicos forma parte del plan de estudios de la carrera en Ingeniería Biomédica con la siguiente competencia general del curso: Utiliza las propiedades de los circuitos RLC para describir la dinámica de sistemas fisiológicos, obtener modelos matemáticos y aplicar el control clásico, esto con el objetivo de integrar los principios de la Ingeniería de Control, la Electrónica Analógica y las Ciencias de la Computación con la Anatomía y Fisiología del cuerpo humano para proporcionar descripciones cuantitativas y cualitativas de sistemas fisiológicos complejos con el objetivo de modelizar, analizar, controlar, ilustrar y predecir su dinámica tanto en el corto como en el largo plazo.

## Objetivos
1. Resolver el sistema de EDOs mediante el metodo de Euler.
2. Graficar el caso con transfusión sanguinea y sin transfusión sanguinea del individuo.

## Descripción detallada del sistema

El siguiente modelo matemático de tres EDOs de primer orden es un modelo mecanicista de compartimento para la eritropoyesis después de la pérdida de sangre en personas sanas, fenómeno que se puede modelizar como un proceso dinámico no lineal. Donde x1(t) representa el compartimento de células precursoras eritroides altamente proliferantes con respecto a la eritropoyetina, x2 (t) describe el compartimento no proliferante de células precursoras
eritroides con respecto a la eritropoyetina, y x3 (t) el compartimento para los eritrocitos maduros y reticulocitos sanguíneos. Con respecto a los parámetros, X0 refleja la cantidad absoluta de células que se destinan al linaje eritroide y que maduran en el primer compartimento de células precursoras eritroides. Las tasas de transición y las tasas de mortalidad entre los compartimentos están dadas por k1, k2 y , estas tasas son independientes de la hormona eritropoyetina. La compensación de la pérdida de sangre se describe mediante un término de retroalimentación de los eritrocitos a las células en proliferación basado en la pérdida fraccional de eritrocitos. Con base en lo anterior, se introducen los parámetros y , que se utilizan para la descripción de las características individuales de la eritropoyesis. Se asume que cada individuo tiene un recuento medio de eritrocitos indicado por el parámetro Base.
El sistema se resolvio con los siguientes parametros de gamma y beta:
1. gamma = [0.769, 0.388, 0.510, 0.590,0.262, 0.324, 0.356, 0.089, 0.243, 0.057]
2. beta = [1.650,0.867,1.617,2.615,1.518,2.676,0.891,2.557,0.925,0.089]
Y con las siguentes condiciones iniciales:;
1. x1(0) = 57.2815   57.2456   57.7344   61.6576   59.1265   56.9357   58.2014   57.6006   58.2847   60.8827;
2. x2(0) = 42.7184   42.6916   43.0562   45.9820   44.0943   42.4605   43.4044   42.9564   43.4666   45.4040;
3. x3(0) = 859.2221  858.6837  866.0163  924.8643  886.8976  854.0354  873.0213  864.0086  874.2705  913.2401;

Palabras clave: Eritropoyesis; Regeneracion de globulos rojos; Modelo matematico; Simulaciones numéricas.

## Lista de archivos incluidos en el repositorio

1. Cuaderno computacional de MATLAB \[.mlx].
2. Imágenes de las simulaciones \[.pdf y .png].

## Referencias

\[1] P. A. Valle, Syllabus para Modelado de Sistemas Fisiológicos, Tecnológico Nacional de México / Instituto Tecnológico de Tijuana, Tijuana, B.C., México, 2025. Permalink: https://biomath.xyz/course/

\[2] M. C. Khoo, Physiological Control Systems Analysis Simulation, and Estimation, 2nd ed. Piscataway, New Jersey, USA: IEEE Press, 2018, Section 4, Page 93.

\[3] M. Tetschke, P. Lilienthal, T. Pottgiesser, T. Fischer, E. Schalk & S. Sager, Mathematical Modeling
 of RBC Count Dynamics after Blood Loss , Processes, vol. 6, issue 9, Sep 2018. https://doi.org/10.3390/pr6090157
