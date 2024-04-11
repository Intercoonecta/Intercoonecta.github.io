# Primeros pasos para los tutoriales

## Introducción

Los hackatones son altamento interactivos gracias al uso de la plataforma JupyterHub


```{admonition} Instrucciones para el uso de la plataforma JupyterHub
- Entrada a la plataforma: https://oceanhackweek.2i2c.cloud
- Para actualizar los tutoriales en la plataforma, [sigan estas instrucciones](https://intercoonecta.github.io/primeros-pasos.html#como-consigo-el-repositorio-de-los-tutoriales-en-el-hub)
- Favor cerrar la sesión cuando termine de usarla por el día
  - Python: `Archivo > Panel de Control`, luego presione `Stop My Server` y `logout`
  - R: Presione el enlace https://oceanhackweek.2i2c.cloud/hub/home, y luego presione `Stop My Server` y `logout`
```

Los tutoriales se ejecutarán en vivo en el [JupyterHub  del hackatón ("El Hub"), https://oceanhackweek.2i2c.cloud](https://oceanhackweek.2i2c.cloud) en su navegador, ya sea como _Jupyter notebooks_ o como _scripts_ y _notebooks_ en `RStudio`. El/la instructor/a y todas las personas que participen pueden estar ejecutando sus propias copias del tutorial en su cuenta del Hub, con archivos clonados desde la fuente en `GitHub`.

A continuación hay instrucciones para iniciar los tutoriales en el Hub en su navegador y actualizar los archivos de los tutoriales con la última versión del repositorio de tutoriales `GitHub`, [https://github.com/Intercoonecta/tutoriales](https://github.com/Intercoonecta/tutoriales).

El calendario de tutoriales está disponible [aquí](tutoriales), y los enlaces a los materiales de los tutoriales y algunos otros recursos estarán disponibles allí también.

## ¿Cómo consigo el repositorio de los tutoriales en el Hub?

Para los tutoriales, recomendamos el uso de [nbgitpuller](https://jupyterhub.github.io/nbgitpuller/) para clonar y extraer el repositorio de los tutoriales, o actualizar la copia que ya tiene. Utilice el enlace mágico `nbgitpuller` a continuación para lograr este clon o actualización.

```{admonition} Haga _pull_ del repositorio de los tutoriales usando la magía de nbgitpuller

El enlace `nbgitpuller` es mágico, pero no puede detectar qué perfil está ejecutando actualmente. Debería o actualizar el (mismo) repositorio de los tutoriales, pero podría dar un error si utiliza el enlace de Python si está utilizando activamente el perfil R, o al revés.

::::{tab-set}

:::{tab-item} Python

[Haga pull del repositorio de los tutoriales para el perfil de Python](https://oceanhackweek.2i2c.cloud/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2FIntercoonecta%2Ftutoriales&urlpath=lab%2Ftree%2Ftutoriales)

:::

:::{tab-item} R

[Haga pull del repositorio de los tutoriales para el perfil de R](https://oceanhackweek.2i2c.cloud/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2FIntercoonecta%2Ftutoriales&urlpath=rstudio)

:::

::::

```

Vea esta [discusión extendida (en inglés)](https://oceanhackweek.org/resources/prep/jupyterhub.html#how-do-i-get-the-tutorial-repository) para más detalles sobre `nbgitpuller` y el enfoque alternativo basado en comandos `git` y los flujos de trabajo `GitHub`.
