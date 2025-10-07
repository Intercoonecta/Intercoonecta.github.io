# Primeros pasos para el Taller Intermedio

## Introducción

Nuestros tutoriales son altamente interactivos gracias al uso de la plataforma [JupyterHub](JupyterHub).

```{admonition} Instrucciones para el uso de nuestra plataforma JupyterHub
- Entrada a la plataforma: https://oceanhackweek.2i2c.cloud
- Para actualizar los tutoriales en la plataforma, [sigue estas instrucciones](#como-cargar-el-repositorio-de-los-tutoriales-al-hub)
- Por favor cierra la sesión cuando termines de usarla por el día
  - **Python:** `Archivo > Panel de Control`, luego presiona `Stop My Server` y `logout`
  - **R:** Presiona el enlace https://oceanhackweek.2i2c.cloud/hub/home, y luego presiona `Stop My Server` y `logout`
  - Ver [aquí para instrucciones más detalladas](hub:cerrar-sesion)
```

Los tutoriales se ejecutarán en vivo en el [JupyterHub de OceanHackWeek (**"El Hub"**, https://oceanhackweek.2i2c.cloud](https://oceanhackweek.2i2c.cloud)) en tu navegador, ya sea como _Jupyter notebooks_ o como _scripts_ y _notebooks_ en `RStudio`. Él/la instructor/a y todas las personas que participen pueden estar ejecutando sus propias copias del tutorial en su cuenta del Hub al mismo tiempo, con archivos clonados desde la fuente en `GitHub`, https://github.com/Intercoonecta/Talleres_intermedios. Nuestra página [JupyterHub](JupyterHub) contiene instrucciones detalladas sobre el uso del Hub.

El calendario de tutoriales está disponible [aquí](tutorialesintermedios2025), y los enlaces a los materiales de los tutoriales y algunos otros recursos estarán disponibles allí también.

(hub-cargartutoriales:taller-intermedio)=
## Cómo cargar el repositorio de los tutoriales al Hub

Hacemos uso de la herramienta [nbgitpuller](https://jupyterhub.github.io/nbgitpuller/) para clonar y extraer el [repositorio de los tutoriales](https://github.com/Intercoonecta/Talleres_intermedios), o actualizar la copia que ya tienes. Utiliza el enlace apropiado de `nbgitpuller` a continuación para lograr este clon o actualización.

```{admonition} Carga el repositorio de los tutoriales por medio de **nbgitpuller**

El enlace `nbgitpuller` es mágico, pero no puede detectar cual entorno (Python o R) estás ejecutando actualmente. Ambos enlaces, de Python y R, actualizan el mismo repositorio de tutoriales, pero pueden dar un error si utilizas el enlace de Python mientras estás en el entorno de R, o viceversa. Para cargar (subir) o actualizar los tutoriales del repositorio [`Talleres_intermedios`](https://github.com/Intercoonecta/Talleres_intermedios) en tu cuenta en el Hub, presiona la pestaña correspondiente:

::::{tab-set}

:::{tab-item} Python

Presiona este enlace para [hacer un "pull" del repositorio de los tutoriales para el entorno de Python](https://oceanhackweek.2i2c.cloud/hub/user-redirect/git-pull?repo=https://github.com/Intercoonecta/Talleres_intermedios&urlpath=lab/tree/Talleres_intermedios)

:::

:::{tab-item} R

Presiona este enlace para [hacer un "pull" del repositorio de los tutoriales para el entorno de R](https://oceanhackweek.2i2c.cloud/hub/user-redirect/git-pull?repo=https://github.com/Intercoonecta/Talleres_intermedios&urlpath=rstudio)

:::

::::

```
