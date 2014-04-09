---
layout: blog
tittle: Implantación de la infraestructura de prueba OpenStack
menu:
  - Unidad 2
  - Aplicaciones
---
## Introducción a Git

###Contenidos

[Git](http://git-scm.com/) es un software de control de versiones diseñado por Linus Torvalds, pensando en la eficiencia y la confiabilidad del mantenimiento de versiones de aplicaciones cuando estas tienen un gran número de archivos de código fuente. 

[GitHub](https://github.com/) es una forja para alojar proyectos utilizando el sistema de control de versiones Git.

Muchos de los scripts que vamos a usar para implantar la infraestructura de prueba de OpenStack están almacenado en **repositorios** en GitHub, por lo tanto tendremos que clonar dichos repositorios para bajarlos a nuestros equipos.

Cuando se desarrolla utilizando git, lo habitual es ir creando **ramas
(branchs)** independientes para cada funcionalidad. La rama por defecto se
denomina *master* y de ella suelen salir el resto de las ramas en un momento
determinado y se fusionan (*merge*) cuando se termina.

###Prácticas

1. Instala el cliente git

        # apt-get install git

2. Nuestro curso esta almacenado en un repositorio en GitHub, si quieres bajarlo sólo tienes que clonarlo:

        $ git clone https://github.com/iesgn/cloud.git
        
3. Si queremos actualizar nuestro repositorio local con los cambios del repositorio remoto

        $ cd cloud
        $ git pull

4. Cuando trabajemos con OpenShift necesitaremos hacer cambios en el repositorio remoto a partir de nuestro repositorio local, para ello tenemos que ejecutar tres instrucciones:

        $ git add <filename>
        $ git commit -m "Mensaje del commit"
        $ git push

###Enlaces interesantes

* [git - la guía sencilla](http://rogerdudler.github.io/git-guide/index.es.html)
* [Pro Git - Libro de referencia](http://git-scm.com/book)