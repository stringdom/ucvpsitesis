# ucvpsitesis

Formato de estilo LaTeX para la presentación de tesis ante la escuela de psicología de la Universidad Central de Venezuela utilizando referencias bibliográficas al estilo APA.

## Dependencias
El formato requiere una distribución de LaTeX2e. Por ejemplo, [MiKTeX](https://miktex.org/). El estilo asume que está siendo utilizado en un entorno Windows 10 con acceso a la fuente Times News Roman.

* Compilador: Xelatex
* `logo-ucv.jpg` debe encontrarse en la carpeta raíz del proyecto
* Documentclass: memoir

        \documentclass[12pt,letterpaper,twoside,openright,oldfontcommands]{memoir}


## Uso del estilo

En este momento del desarrollo el archivo debe ser descargado y copiado en la carpeta raíz del proyecto LaTeX.

El estilo debe ser invocado con el siguiente comando LaTeX en el archivo `.tex` principal:

    \usepackage{ucvpsitesis}

## Comandos del estilo

### Obligatorios
La presentación correcta del formato de estilo depende del uso obligatorio de los siguientes comandos en el archivo `.tex` principal.

\author
    : Nombre del autor o autores.

\tutor
    : Nombre del tutor de la tesis.

\departamento
    : Nombre del departamento que aprueba la tesis.

\mail
    : Correo electrónico de los autores.

\shorttitle
    : Título corto a ser utilizado en los encabezados de página.

\engtitle
    : Título en Inglés de la tesis

\date
    : Fecha de presentación de la tesis.

## Opcionales

\maketitle
    : El estilo reescribe completamente el comando `maketitle` con las exigencias de formato de la escuela de psicología.

\frontmatter
    : El comando del paquete `memoir` permite formatear correctamente la numeración de las páginas. También permite la creación de elementos especiales como dedicatorias, agradecimientos y resúmenes.

\theauthor
    : Imprime el contenido declarado en `\author`.

\thetitle
    : Imprime el contenido declrada por `\title`.
