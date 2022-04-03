<h1 align="center"> WebScrapping Buscador de másteres </h1>
<h3 align="center"> M2.851 - Tipología y ciclo de vida de los datos (aula 2) -Master en Ciencia Datos </h3>
<h3 align="center"> Autores: </h3>
<h3 align="center"> Almudena Caballero Manzanas </h3>
<h3 align="center"> Ángel A. Urbina Sánchez </h3>
<h5 align="center"> Practica 1 - <a href="https://www.uoc.edu/">Universitat Oberta de Catalunya</a> (Primavera 2022) </h5>


<p>En esta práctica se elabora un caso práctico orientado a aprender a identificar los datos relevantes para un proyecto analítico y usar herramientas de extracción de datos.</p>
<p>Nos planteamos recopilar y almacenar, para posteriormente analizar, la información relativa a las posibles <b>ofertas de estudios de máster</b>.</p>
<p>El objetivo de obtener esta información es el disponer de un único fichero, sin necesidad de visitar cada una de las webs, con la información que consideramos más relevante para elegir el máster considerado.
Elegimos <a href=https://www.emagister.com>Emagister</a>, web buscadora de másteres, y tratamos de obtener toda la información que nos ayude a la elección del máster deseado. </p>
<p>Consideramos que la información relevante para desarrollar esta decisión es:<p>
<ul>
    <li> Descripción del máster: tipología, duración, metodología, …</li>
    <li> Precio</li>
    <li> Requisitos</li>
    <li> A quién va dirigido</li>
    <li> Posible financiación</li>
    <li> Opiniones</li>
</ul>

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

<h2> Consideración Generales</h2>
<p> La estructura de la solución diseñada es modular con el objetivo de simplicar el mantenimiento y el proceso de mejora en futuras versiones.</p>
<p> Para simplificar la identificaciones de posibles bugs e incidencias en la ejecución asi como para favorecer el desarrollo de mejoras sobre el código propuesto se documenta todo el proceso en los diferentes logs. (Terminal & Fichero )</p>
<p> Los pasos considerados han sido</p>
<ul>
    <li><b>Generación Archivo Links</b> Extracción informacion Links de los diferentes masters</li>
    <li><b>Extracción Información Masters</b> Se lee archivo anterior con listado de links de cada master individual. Se extrae la información de cada uno de los Masters</li>
    <li><b>Extracción Imagenes</b> Extracción de información en formato grafico. Se trata de los Logos de las diferentes instituciones que ofrecen cursos.</li>
</ul>

<p> Se han desarrollado dos maneras diferentes de obtención de la informacion de los Masteres:</p>
<ul>
    <li><b>MODO SECUENCIAL</b> El acceso a los diferentes links WEB se desarrolla de forma secuencial (Mayor tiempo de ejecución).</li>
    <li><b>MODO MULTIPROCESO</b> El acceso a los diferentes links WEB se desarrolla de forma paralela (Menor tiempo de ejecución).</li>
</ul>

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

<h2> :floppy_disk: Descripción archivos proyecto</h2>

<p>Este proyecto se ha desarrollado integramente en Python utilizando la herramienta Visual Studio Code. Continene varios archivos en formato notebook, y varios directorios con la siguiente estructura.:</p>
<h4>CODIGOS:</h4>
<ul>
  <li><b>PRA01.ipynb</b> - Contiene todo el código Python del WebScraping desarrollado.(Formato Notebook Python)</li>
  <li><b>loggingUOCPRA01.conf</b> - Archivo Auxiliar de configuración de loggins para el archivo Python anterior. (Formato txt)</li>
  <li><b>UOCPRA01.log</b> - Archivo auxiliar log en formato .txt resultado de la ejecución del archivo python.</li>
</ul>

<h4>RESULTADOS:</h4>
<ul>
  <li><b>RESULT-27-03-22.xlsx</b> - Contiene la información extraida de la Web en formato (.xlsx).</li>
  <li><b>RESULT-27-03-22.csv</b> - Si existe. Contiene la información extraida de la Web en formato (.csv).</li>
</ul>

<h4>IMAGENES:</h4>
<ul>
  <li><b>XXXXXX.jpg</b> - Conjunto de Archivos de Imagenes Descargados (.jpg).</li>
  <li><b>XXXXXX.png</b> - Conjunto de Archivos de Imagenes Descargados (.png).</li>
</ul>

<h4>DESCRIPCION:</h4>
<ul>
  <li><b>M2851_PRA1.docx</b> - Incluye el contenido de la practica en formato (.docx)</li>
  <li><b>M2851_PRA1.pdf</b> - Incluye el contenido de la practica en formato (.pdf)</li>
</ul>

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

<!-- CREDITS -->
<h2 id="credits"> :scroll: Creditos</h2>

Agradecemos a los diferentes autores de las siguientes referencias el habernos facilitado el trabajo de desarrollo:

<ul>
  <li>https://stackoverflow.com/questions/66876071/extracting-a-complex-substring-using-regex-with-data-from-a-string-in-python</li>
  <li>https://stackoverflow.com/questions/14473180/regex-to-get-a-filename-from-a-url</li>
  <li>https://medium.com/@kunal.rustagi/boost-your-web-crawler-using-multiple-processes-in-python-3cc3ff519226</li>
  <li>https://coderzcolumn.com/tutorials/python/logging-config-simple-guide-to-configure-loggers-from-dictionary-and-config-files-in-python</li>
</ul>

