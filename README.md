# Pacman-python-300519
## Install Pacman for python 2.7 in linux.
*Link de descaga de la maquina virtual utilizada, motada en VirtualBox (archivo vdi):
*https://drive.google.com/open?id=1GfllUJp40ncROwviZAy3SbxPCIkymJsF

#### Abstract – Pac-Man is without a doubt the most recognizable character throughout video games. The bestselling coin-op in history, it has also been ported to just about every gaming platform over the past 22 years. Nowadays we can play this game in any platform that we own. The project pretend mixing this game with Python, working in any Linux distribution, for that, I want to make the installation process easier, using shell scripts, then, learn Python using their tools in a game.
### Introducción
El siguiente proyecto va a consistir en generar un Shell Script que sea capaz de instalar todos los módulos necesarios para la correcta ejecución de Pacman, además de que se busca aprender de estos módulos, interviniendo un poco en el código del juego.
Todo el proyecto se estará trabajando en la version 2.7 de Python.
### Desarrollo
Se requiere poner en contexto de todas las librerías que se utilizan para poder ejecutar Pacman con Python y Tensorflow, por lo que
* Python
Python es uno de los lenguajes de programación dinámicos más populares que existen entre los que se encuentran Perl, Tcl, PHP y Ruby. Aunque es considerado a menudo como un lenguaje "scripting", es realmente un lenguaje de propósito general. En la actualidad, Python es usado para todo, desde simples "scripts", hasta grandes servidores web que proveen servicio ininterrumpido 24x7. Es utilizado para la programación de interfaces gráficas y bases de datos, programación web, tanto en el cliente como en el servidor y "testing" de aplicaciones. Además, tiene una amplia aceptación por científicos que hacen aplicaciones para los supercomputadores más rápidos del mundo y por los niños que recién están comenzando a programar.
* Tensorflow
Es una biblioteca de código abierto que se basa en un sistema de redes neuronales. Esto significa que puede relacionar varios datos en red simultáneamente, de la misma forma que lo hace el cerebro humano. Por ejemplo, puede reconocer varias palabras del alfabeto porque relaciona las letras y fonemas. Otro caso es el de imágenes y textos que se pueden relacionar entre sí rápidamente gracias a la capacidad de asociación del sistema de redes neuronales. En el programa, se almacenan todas las pruebas y experimentos que se
realizaron para el desarrollo de programas y aplicaciones.
* NumPy
Es una extensión de Python, que le agrega mayor soporte para vectores y matrices, constituyendo una biblioteca de funciones matemáticas de alto nivel para operar con esos vectores o matrices
* Pip
Es un sistema de gestión de paquetes utilizado para instalar y administrar paquetes de software escritos en Python. Muchos paquetes pueden ser encontrados en el Python Package Index (PyPI). Python 2.7.9 y posteriores (en la serie Python2), Python 3.4 y posteriores incluyen pip (pip3 para Python3) por defecto.
* Scikit-image
Es una colección de algoritmos que son utilizados para el procesamiento de imágenes con Python.
* Pythondev Archivos de encabezado, una biblioteca estática y herramientas de desarrollo para construir módulos de Python, extender el intérprete de Python o incrustar Python en las aplicaciones
* TFLearn
Es una biblioteca de aprendizaje profundo modular y transparente construida sobre Tensorflow. Fue diseñado para proporcionar una API de nivel superior a TensorFlow con el fin de facilitar y acelerar las experimentaciones, mientras se mantiene completamente transparente y compatible con él.
* Apt
APT (Advanced Package Tool) Es la herramienta de línea de comando para interactuar con los paquetes del Sistema.
Cada uno de estos módulos son necesarios para la ejecución de un proyecto ya antes realizado PacManLearning el cual cuenta con el juego, y algunos elementos para poder aprender de él. Además, propone algunas actividades para que el usuario se vaya familiarizando con los módulos que este proyecto contiene.
El Shell Script contiene varias líneas que serán explicadas a continuación:
• mkdir /home/usr/Desktop/Virtualenvi
La cual generará una carpeta en donde se creará un sistema virtual que albergará todos los módulos próximos a instalarse.
• python --version
• Que Indica la versión de Python que se tiene instalada, también se realiza esta acción para ver la versión de Pip y virtualenv.
• virtualenv Virtualenvi -p python2.7
• Esta línea genera el entorno virtual en donde estarán instalados los módulos que se utilizarán próximamente.
• source Virtualenvi/bin/activate
Este comando es utilizado para trabajar en el entorno virtual antes creado.
• sudo apt update
Utilizado para instalar una nueva version de apt
• sudo apt install python-dev python-pip Comando utilizado para instalar pip
• sudo apt-get install python-dev Comando utilizado para instalar python-dev
• pip install --upgrade pip Utilizado para actualizar el comando pip a una version más reciente.
• pip install --upgrade http://storage.googleapis.com/tensorflow/mac/cpu/tensorflow-1.0.1-py2-none-any.whl Este comando permite descargar e instalar Tensorflow.
• pip show tensorflow Comando que permite mostrar módulos instalados por pip
• export PYTHONPATH=/home/osboxes:$PYTHONPATH
• pip install scikit-image Permite instalar Scikit-Image
• pip install --upgrade scikit-image Permite actualizar el modulo anterior
• pip install tflearn Permite instalar tflearn
• pip list Comando que permite visualizar todos los paquetes instalados con pip
• echo "Para descargar Pacman ingrese a este link https://github.com/upslp-teoriacomputacional/Pacman-python-300519" Comando que imprime la localidad del juego para descargarse.
• pip install pacman-game A modo de prueba se instaló otro juego de Pacman esta vez en forma de matriz en la misma consola.
• deactivate Permite salir del entorno virtual en el que se está trabajando.
Una vez instalados los módulos se prosigue a correr el juego, pero existe un error en el código del juego el cual no permite ejecutarse. Se mandan errores de sintaxis algo que ya no se tiene en nuestro control
### Conclusiones
Debido a algunas complicaciones con el juego como tal, no se pudo llegar a correr debido a que tenía errores de sintaxis algo que se debe de revisar minuciosamente todo el código para poder determinar la falla.
#### Referencias
Francisco José Fernández Jiménez, F. J. (2018). Programación Shell-script en Linux. Obtenido de Departamento de Ingeniería Telemática (DIT): http://trajano.us.es/~fjfj/shell/shellscript.htm#_Toc444081192
Grandio, X. (14 de Julio de 2017). Qué es Tensor Flow: aplicaciones del sistema de inteligencia artificial de Google. Obtenido de Marketing 4 Ecomerce: https://marketing4ecommerce.net/tensorflow-que-es-y-sus-aplicaciones/
Image processing in Python. (s.f.). Obtenido de https://scikit-image.org/
Install TensorFlow with pip. (s.f.). Obtenido de Tensorflow: https://www.tensorflow.org/install/pip?lang=python2
Kolekar, P. (s.f.). pacman-game 1.0.3.dev1. Obtenido de Pypi: https://pypi.org/project/pacman-game/
Package: python-dev (2.7.9-1). (s.f.). Obtenido de Debian: https://packages.debian.org/es/jessie/python-dev
pip - The Python Package Installer. (6 de Mayo de 2019). Obtenido de https://pip.pypa.io/en/stable/
TFLearn: Deep learning library featuring a higher-level API for TensorFlow. (s.f.). Obtenido de http://tflearn.org/
TravisOliphant. (20 de Julio de 2007). History of SciPy. Obtenido de SciPy: https://web.archive.org/web/20070927015018/http://www.scipy.org/History_of_SciPy/
Venners, B. (13 de Enero de 2003). The Making of Python. Obtenido de Artima: https://www.artima.com/intv/pythonP.html
