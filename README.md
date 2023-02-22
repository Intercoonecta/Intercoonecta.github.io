# Hackaton OHW en español

*(Este texto es preliminar. Lo puliré y ampliaré luego)*

Con el [Jupyter Book](https://jupyterbook.org) (y muchos sistemas parecidos), uno modifica los archivos "fuente", típicamente en markdown, y luego "genera" los archivos del sitio en sí. Pueden leer sobre esto [aquí](https://jupyterbook.org/en/stable/basics/building/index.html). 

Los archivos fuente (el contenido) se almacenan en el branch principal, `main`, bajo la carpeta [`sitio`](sitio). Los archivos generados del sitio son colocados en el branch `gh-pages`. En la gran mayoría de los casos no es recomendable editar los archivos en `gh-pages` manualmente, directamente. Entonces, hay dos workflows recomendados:
- Se corre (`build`) jupyter book localmente, para confirmar que todo se vea bien. Una vez que esté listo, se empujan los archivos del build al repositorio usando el programa ghp-import, corrido con algo parecido a esto: `ghp-import -n -p -f --remote upstream sitio/_build/html`. Los archivos fuente en el repositorio son actualizados usando idealmente un pull request. Esto es lo que he estado haciendo hasta ahora.
- Activando un sistema en GitHub que genera (build) el sitio automáticamente cada vez que se envía un pull request. Este sistema también incluye un preview de los cambios propuestos, que es muy útil. Este automatización hace futuras modificaciones mucho más sencillas, especialmente cuando se trata de modificaciones de páginas existentes.

Este mecanismo automático ya está activo. Ahora, al crear un pull request (PR), después de un minuto (mas o menos) verán un enlace como este bajo "Deploy Preview for sage-puppy-e64764 ready!":
![image](https://user-images.githubusercontent.com/742403/220565139-f8aea2b4-9801-4ef0-81e8-9a5e318d3a4d.png)

Este enlace los llevará a una versión temporal del sitio donde pueden confirmar los cambios propuestos en el PR. Una vez que le hagan "merge" al PR, el sitio será reconstruido automáticamente en `gh-pages` con los cambios en el PR. Esto toma un par de minutos.

Pueden ver un ejemplo de esto en un PR reciente, como este: #3

Es sencillo editar una página directamente desde el sitio web: en los íconos arriba a la derecha de cada página, presionen el ícono de gihub y luego seleccionen "suggest edit". Esto los lleva a github, con el interfaz de modificación del markdown. 
![image](https://user-images.githubusercontent.com/742403/220717342-8afb20b4-5ee4-4547-9c92-c5011633431b.png)

Cuando estén listos a enviar los cambios, por favor seleccionen "Create a new branch for this commit and start a pull request" antes de presionar "Commit changes". Esto nos permitir a otros revisar los cambios antes de aprobarlos.

![image](https://user-images.githubusercontent.com/742403/220717826-e1062654-4757-4bcb-9d85-aa8300dcf432.png)


Hay dos archivos importantes de configuración del sitio:
- [`_config.yml`](sitio/_config.yml). [Configuraciones básicas del sitio](https://jupyterbook.org/en/stable/customize/config.html). Raremente tendremos que modificar esto.
- [`_toc.yml`](sitio/_toc.yml). "Table of Content". [Organización de las páginas en el sitio.](https://jupyterbook.org/en/stable/basics/organize.html)
