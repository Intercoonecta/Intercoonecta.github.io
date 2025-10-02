# JupyterHub: Acceso a JupyterLab y RStudio en la nube

## ¿Qué es Jupyter?

[Jupyter](https://es.wikipedia.org/wiki/Proyecto_Jupyter) es un ecosistema abierto (*open source*) de computación desarrollado por el [Proyecto Jupyter](https://jupyter.org/) que incluye herramientas para el desarrollo, intercambio y presentación interactiva de código y proyectos de análisis de datos, con apoyo para una gran cantidad de lenguajes de programación (su nombre se deriva de los lenguajes de código abierto Julia, Python y R).

### Más información, instrucciones y tutoriales sobre Jupyter

Consulta [nuestro tutorial sobre Jupyter del programa "Aula Invertida"](https://github.com/Intercoonecta/Aula-invertida/blob/main/Intro-a-Jupyter/Jupyter.md). Este tutorial incluye una reseña del uso de cuadernos Jupyter, [**instrucciones para cambiar el interfaz de JupyterLab al español**](https://github.com/Intercoonecta/Aula-invertida/blob/main/Intro-a-Jupyter/jupyter-tutorial.md#cambiar-el-interfaz-al-espa%C3%B1ol), e instrucciones para instalar JupyterLab en tu computadora.

[Aquí puedes acceder a un video en YouTube grabado durante el "Taller Intermedio"](https://youtu.be/SP3SnrQ2HTY?feature=shared&t=818), cuando cubrimos el tutorial de JupyterHub -- el material abarcado en esta página.

```{admonition} Presiona aquí para leer más sobre el "ecosistema" de Jupyter
:class: dropdown

El ecosistema del Proyecto Jupyter está compuesto de tres elementos (ver [*"2.2 But first, what is Jupyter Notebook?"*](https://jupyter4edu.github.io/jupyter-edu-book/why-we-use-jupyter-notebooks.html#but-first-what-is-jupyter-notebook)): una colección de estándares, una comunidad y una serie de herramientas de software. [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/) es una aplicación para crear, manejar y correr cuadernos (*notebooks*) Jupyter. Un [cuaderno Jupyter](https://es.wikipedia.org/wiki/Proyecto_Jupyter#Jupyter_Notebook) es un documento que permite mezclar código ejecutable, ecuaciones, visualizaciones y texto narrativo formateado. Un cuaderno puede combinar en un sólo documento el código, los datos que utiliza y sus resultados, incluyendo explicaciones, gráficas y contenido multimedia, de tal modo que pueda ser compartido ampliamente y ejecutado por otros con relativa facilidad. El cuaderno permite la creación de narrativas computacionales interactivas y reproducibles.

El ecosistema Jupyter utiliza tecnología web que permite correr las aplicaciones en un navegador (*browser*) web con las computaciones ya sea en tu propia computadora ("local") o a través de servicios o servidores remotos, incluyendo en la nube. Los cuadernos Jupyter y el ecosistema Jupyter hoy en día gozan de una gran popularidad en aplicaciones de ciencias de datos y aplicaciones científicas en general, especialmente con el lenguaje Python.

```

## Entorno computacional compartido, en la nube

Enseñar software a un grupo diverso de participantes, cada uno/a con diferentes computadoras y sistemas operativos, es un desafío. Tenemos formas específicas de configurar nuestro software para que los tutoriales sean exitosos, por lo que lleva tiempo configurarlos todos de manera consistente. Nuestra solución a este reto es brindarles a los/as participantes de eventos del *OceanHackWeek en español* acceso a un entorno de computación en la nube preconfigurado para el software específico que implementamos, y con flexibilidad para el desarrollo de proyectos de equipo. Se accede a este entorno de computación en la nube desde cualquier navegador web, lo que elimina la necesidad (¡y complicación!) de configurar la computadora individual de cada persona con las bibliotecas, dependencias y aplicaciones necesarias.

En este entorno compartido, cada usuario tiene su propia cuenta pre-configurada a los mismos entornos de Python y R y acceso a recursos computacionales idénticos. Este entorno global está basado en el sistema [JupyterHub](https://jupyter.org/hub) (parte del ecosistema Jupyter), el cual nos permite comenzar a trabajar rápidamente con código sin perder tiempo configurando la computadora de cada quien. **JupyterHub da acceso tanto a la aplicación `JupyterLab` para programar en Python (y otros lenguajes) como a la aplicación [`RStudio`](https://es.wikipedia.org/wiki/RStudio) para R. Utilizaremos estas dos aplicaciones para seguir y correr los tutoriales.**

Te recomendamos que utilices nuestros recursos compartidos de JupyterHub para ejecutar todos los tutoriales y para trabajar en tus proyectos. También esperamos que practiques la instalación de bibliotecas de Python y R localmente en tu propia computadora para que puedas continuar trabajando después que concluya nuestro evento.


## Acceso a "El Hub", nuestro entorno compartido en la nube

Es fácil acceder a nuestro entorno computacional de JupyterHub en la nube (**"El Hub"**). Dirígete a [https://oceanhackweek.2i2c.cloud](https://oceanhackweek.2i2c.cloud) en tu navegador:

![hub-opening](/imagenes/jupyterhub/ohwe24-jupyterhub-opening.png)

Ahora presiona el botón "Log in para continuar", y la siguiente pantalla te pedirá tu nombre de usuario y contraseña de tu cuenta de GitHub para entrar con tus credenciales de GitHub:

![sign-in with github](/imagenes/jupyterhub/2i2chub-signin-with-github.png)

Presiona el botón "Sign in". **La siguiente pantaya sólo aparecerá la primera vez que entres al Hub.**

```{admonition} Presiona aquí para ver esa pantaya, con instrucciones
:class: dropdown

Esta te pide otorgar el permiso requerido a nuestro sistema de JupyterHub para combrobar tu identidad con GitHub. Presiona el botón "Authorize 2i2c-org":

![authorize 2i2c](/imagenes/jupyterhub/2i2chub-authorize-github-access.png)
```

### ¡Ya estás adentro!

Ahora sólo falta seleccionar el lenguaje de programación y la aplicación que deseas usar en la sesión actual: "Python en JupyterLab" o "R en RStudio"

![hub select Python or R](/imagenes/jupyterhub/ohwe24-jupyterhub-select-Python-or-R.png)

Una vez hecha la selección, verás una notificación como esta mientras el entorno de JupyterHub está cargando:

![hub-loading](/imagenes/jupyterhub/ohwe24-jupyterhub-loading.png)

Tomará un poco de tiempo en cargar y estar listo, especialmente la primera vez. ¡Ten paciencia! Una vez que esté listo:

```{admonition} ¿Seleccionaste *Python* o *R*? Presiona la pestaña correspondiente

::::{tab-set}

:::{tab-item} Python -> JupyterLab

 **Si seleccionaste "Python"**, verás tu propia instancia de **JupyterLab** (con interfaz en inglés):

![JupyterLab - inglés](/imagenes/jupyterhub/ohwe24-jupyterhub-Python-jupyterlab-eng.png)

Y al [cambiar el idioma del interfaz a español](https://github.com/Intercoonecta/Aula-invertida/blob/main/Intro-a-Jupyter/jupyter-tutorial.md#cambiar-el-interfaz-al-espa%C3%B1ol):

![JupyterLab - español](/imagenes/jupyterhub/ohwe24-jupyterhub-Python-jupyterlab-es.png)

:::

:::{tab-item} R -> RStudio

**Si seleccionaste R,** verás tu propia instancia de **RStudio** (con interfaz en inglés):

![RStudio](/imagenes/jupyterhub/ohwe24-jupyterhub-R-RStudio.png)

:::

::::

```


## Cómo cargar el repositorio de los tutoriales al Hub

Hacemos uso de la herramienta [nbgitpuller](https://jupyterhub.github.io/nbgitpuller/) para clonar y extraer el repositorio de los tutoriales, o actualizar la copia que ya tienes. `nbgitpuller` se aplica a través de un enlace especial, adaptado a un repositorio específico y al entorno o de Python o de R. 

Instrucciones y enlaces específicos se encuentran bajo cada evento:
- [Instrucciones para el **Taller Intermedio**](hub-cargartutoriales:taller-intermedio)
- [Instrucciones para el **Hackatón**](hub-cargartutoriales:hackaton)

### Alternativa con comandos de `git` (¡con cuidado!)

`Nbgitpuller` es genial, porque incorpora ("merge") automáticamente cualquier cambio hecho en el Hub con cambios ocurridos en repositorio fuente cuando presionas el enlace de nueva, utilizando una [serie de reglas básicas (enlace en inglés)](https://jupyterhub.github.io/nbgitpuller/topic/automatic-merging.html#topic-automatic-merging).

Puedes obtener el mismo resultado que `nbgitpuller` utilizando `git` directamente, pero puede requerir una combinación complicada de `git add`, `git stash`, `git pull`, y `git stash apply` para retener tus cambios junto con los cambios hechos en el repositorio fuente.

**¡Atención!** Si comienzas utilizando el enlace de `nbgitpuller` y luego tratas de cambiar al uso de `git` directamente, cuando trates de usar el enlace de `nbgitpuller` de nuevo es muy probable que te encuentres con [resultados impredecibles (enlace en inglés)](https://jupyterhub.github.io/nbgitpuller/#when-to-use-nbgitpuller). Esto puede ser corregido borrando, moviendo o cambiando el nombre del directory de los tutoriales y utilizando `nbgitpuller` de nuevo.


(hub:cerrar-sesion)=
## Cierra tu sesión en el Hub cada día

**Es muy importante cerrar la sesión en el Hub cuando termines de usarla por el día o por un período prolongado.** Esto nos ayuda a reducir el costo de la infraestructura en la nube.

```{admonition} Presiona la pestaña correspondiente a la sesión (entorno) que estás usando actualmente

::::{tab-set}

:::{tab-item} Python / JupyterLab

Accede al menú `Archivo > Panel de Control`:

![hub shut down step 1](/imagenes/jupyterhub/ohwe24-shutdownhub-step1.png)

luego presiona el botón `Stop My Server` y el enlace `logout` arriba a la derecha.

![hub shut down step 2](/imagenes/jupyterhub/ohwe24-shutdownhub-step2.png)

El menú `Archivo > Cerrar sesión` en realidad no cierra la sesión del Hub, así que por favor sigue estos pasos.

:::

:::{tab-item} R / RStudio

Los menús `File > Log out` y `File > Quit session` en realidad no hacen nada! Presiona el enlace https://oceanhackweek.2i2c.cloud/hub/home, y luego presiona el botón `Stop My Server` y el enlace `logout` arriba a la derecha, como mencionamos en las instrtucciones de Python.

![hub shut down step 2](/imagenes/jupyterhub/ohwe24-shutdownhub-step2.png)

:::

::::

```


### No perderás tu trabajo

Cerrar la sesión del Hub (`Stop My Server`) **NO** causará la pérdida de tu trabajo o archivos que has creado. Simplemente apaga algunos recursos computacionales. Es equivalente a apagar tu computadora al final del día.
