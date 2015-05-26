# Waterpy #

Simulación de Redes de Agua

Las simulaciones en redes de distribución de agua son usadas para predecir respuestas de un sistema bajo una amplia gama de condiciones sin interrumpir el sistema real.
Actualmente, se dispone de excelentes modelos matemáticos y de eficaces programas de computadoras para simular el trabajo de las redes de distribución de agua. Estas herramientas son ayudas importantes para el planeamiento y diseño de un sistema.
Los modelos matemáticos que existen en la actualidad representan los diferentes métodos de análisis y diseño de redes de distribución de agua, los cuales se basan en ecuaciones y algoritmos.
El modelo de simulación de redes de distribución de agua Waterpy se basó en el análisis de redes de tuberías cerradas, utilizando para su estudio y diseño el Método del gradiente hidráulico.
Waterpy modeliza tres elementos hidráulicos: depósitos, tuberías, y nodos.

Waterpy se programó bajo la plataforma Windows XP, utilizando como lenguaje de programación Python versión 2.6. Además se utilizó un conjunto de bibliotecas de código abierto, para facilitar el procedimiento de cálculo y generación de reportes.

<b>Características del Programa</b>

Consta de un programa principal llamado Waterpy, del cual se derivan dos subprogramas llamados util y redes. En cuanto a los archivos de datos de entrada se tienen dos, uno fijo denominado datos, el cual contiene los valores de la rugosidad absoluta (ks) para diferentes materiales utilizados en la fabricación de tuberías, y el otro bajo el nombre que le asigne el usuario, el cual contiene los argumentos de definición de la red.


<b>Requisitos</b>

<p>Antes de utilizar Waterpy se debe instalar python y las bibliotecas descritas a continuación:</p>

<p>1) Python<br>
Se utilizó la versión 2.6 de python, como ya se dijo para ambiente Windows. Python puede ser descargado de la siguiente dirección:<br>
<a href='http://www.python.org'>http://www.python.org</a></p>

<p>2) Numpy<br>
Es la biblioteca matemática empleada por waterpy para almacenar todas las matrices y vectores, y realizar el cálculo matricial y numérico. La versión utilizada para esta versión de waterpy fue la 1.5.1, la cual se puede descargar de la siguiente dirección:<br>
<a href='http://numpy.scipy.org'>http://numpy.scipy.org</a></p>

<p>3) Reportlab<br>
Es una biblioteca de generación de reportes, utilizada por waterpy para guardar las salidas en formato PDF. La versión de reportlab que se usó para esta versión de waterpy fue la versión 2.5, se puede descargar de la siguiente dirección:<br>
<a href='http://www.reportlab.com/software/opensource/'>http://www.reportlab.com/software/opensource/</a></p>

<p>4) Matplotlib<br>
Es una biblioteca utilizada para la generación de gráficas 2D. Se utilizó la versión 1.0.0, la cual puede ser descargada de la siguiente dirección:<br>
<a href='http://matplotlib.sourceforge.net'>http://matplotlib.sourceforge.net</a></p>

<p>5) Networkx<br>
Es una biblioteca utilizada para la creación y manipulación de grafos y redes. La versión utilizada fue la 1.3, que puede ser descargada de la siguiente dirección:<br>
<a href='http://networkx.lanl.gov'>http://networkx.lanl.gov</a></p>

<p>Para generar la documentación del programa se utilizó Epydoc, para lo cual se requiere la instalación de:</p>

<p>1) Graphviz<br>
Graph Visualization Software) es la biblioteca utilizada por EpyDoc para la generación de grafos, que utiliza el lenguaje DOT. La versión de Graphviz utilizada fue la 2.26.3, que se puede descargar de la siguiente dirección:<br>
<a href='http://www.graphviz.org'>http://www.graphviz.org</a></p>

<p>2) Docutils<br>
Es un sistema de tratamiento de texto de origen abierto para procesar la documentación en formatos útiles, como HTML o Látex.La versión utilizada de docutils fue la 0.5 y se puede descargar de la siguiente dirección:<br>
<a href='http://docutils.sourceforge.net'>http://docutils.sourceforge.net</a></p>

<p>3) Epydoc<br>
La versión utilizada de Epydoc fue la versión 3.0.1. Esta versión no es compatible con las versiones 0.6 y 0.7 de docutils. Se puede descagar de la siguiente dirección:<br>
<a href='http://epydoc.sourceforge.net/'>http://epydoc.sourceforge.net/</a></p>

<b>Implementación</b>

<p>Una vez que se tiene el archivo de datos con los argumentos que defienen la red en estudio, se deben identificar los parámetros del modelo asociados a los argumentos pasados por línea de comandos.</p>

<p>-r Archivo de entrada donde se encuentran los datos de la red (el nombre del archivo lo indica el usuario).</p>
<p>-m material con el cual está construida la tubería (dependiendo de este material, el coeficiente de rugosidad de la tubería varia; estos valores se encuentran en el archivo de entrada llamado ¨datos¨)</p>
<p>-i número de iteraciones a realizar</p>
<p>-p precisión requerida por el usuario</p>
<p>-d número de decimales a mostrar por pantalla</p>
<p>-o mostrar resultados en formato de Imagen y HTML.</p>
<p>-v mostrar información por pantalla</p>

<p>Para iniciar el proceso de cálculo introducimos los parámetros del modelo por línea de comandos, como se muestra a continuación:</p>
<p>c:\...waterpy.py -r redentrada.txt -m pvc -d 3 –o html –v</p>

<p>donde:<br>
[…] indica la ubicación del archivo de entrada en la pc.</p>



