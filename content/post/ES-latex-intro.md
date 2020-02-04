+++
title = "LaTeX Intro (ES)"
date = 2018-08-15T17:11:08-05:00
draft = false
math = true

# Tags and categories
# For example, use `tags = []` for no tags, or the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = ["LaTeX"]
categories = ["short-tutos"]

# Featured image
# Place your image in the `static/img/` folder and reference its filename below, e.g. `image = "example.jpg"`.
[header]
image = ""
caption = ""

+++

## ¿Qué es LaTeX?

$\LaTeX$ es un lenguaje de marcado, muy útil para la creación de documentos científicos.

Una de las ventajas de utilizar LaTeX es que tanto el contenido y su apariencia se manejan—en cierto modo—por separado. Así puedes enfocarte en lo más importante.
Una gran cantidad de revistas científicas, conferencias e incluso universidades tienen *templates* en formato $\TeX$ para que sólo te preocupes por escribir.

Para aprender más del proyecto en general, puedes visitar la **[página oficial](https://www.latex-project.org/about/)**.

## Disclaimer

Antes de comenzar, es importante que sepas que no es un camino fácil. Puedes usar LaTeX para hacer cartas, tesis, ensayos, artículos, libros e incluso presentaciones. Todo esto se hace en un editor de texto y es un proceso ligeramente parecido al de programar—no hay *what you see is what you get*, naturalmente.
Por lo mismo, puede llegar a ser complicado al principio, pero una vez que te acostumbres, el proceso de escritura puede llegar a ser mucho más rápido que preparar un manuscrito en *Word* o algún programa similar.

---

### Editores para empezar

La manera más sencilla de empezar a escribir tus documentos en LaTeX es usando algún proveedor de servicios en línea para ello. Los más famosos son **[ShareLaTeX](https://sharelatex.com)** y **[Overleaf](https://www.overleaf.com/)**, que incluyen un editor amigable y con *preview* instantáneo.
Ambas páginas incluyen también recursos generales en su centro de ayuda, así como *templates* que puedes utilizar para no comenzar desde cero. Recomiendo mucho los revises.

Si quieres intentar correrlo en tu computadora, te recomiendo que busques sobre **[TeX Live](https://www.tug.org/texlive/)** o **[MiKTeX](https://miktex.org/)**. Aunque cada paquete trae un editor, recomiendo que revises si hay algún complemento que pueda encargarse del *highlighting* y la compilación en el editor de texto de tu preferencia.

## Sintaxis y flujo de trabajo

En general, en $\LaTeX$ utilizamos **comandos** que son siempre de la misma forma:

```latex
\commandname[option1,option2,...]{parameter1}{parameter2}{...}
```
Los comandos empiezan con un **backslash** `\`, seguidos por el **nombre del comando**. Si el comando puede recibir **opciones**, se especifican entre corchetes seguidos del nombre del comando. Los **parámetros** van después, cada uno entre llaves.

Por ejemplo, el comando `\textbf{Hola Pueblo}` genera $\textbf{Hola Pueblo}$. `textbf` significa *text in bold face*, es decir, texto en negritas. Hay también `\textit{Hola Pueblo}`, `\texttt{Hola Pueblo}`. Estos comandos generan $\textit{Hola Pueblo}$ y $\texttt{Hola Pueblo}$ respectivamente.

### Entornos

Un **entorno** en LaTeX determina un área que se comporta de cierta manera. Para declarar un entorno, utilizamos los comandos `begin` y `end`:

```latex
\begin{environmentname}
    content goes here
    many lines can go here
    it is a multi line environment
\end{environmentname}
```

Las **listas numeradas**, por ejemplo, se generan en LaTeX con el entorno `enumerate`:

```latex
\begin{enumerate}
    \item First item
    \item Second item
    \item Third item
\end{enumerate}
```

De manera similar, una **lista no numerada** se genera con `itemize`. Existen muchos otros entornos importantes, por ejemplo `document`, el cual encasilla al documento completo.

### Expresiones matemáticas

Probablemente el fuerte de este lenguaje sea el manejo de símbolos matemáticos. Por ejemplo, la expresión $\int (2x^3 + 58x + 29)\text{d}x$ se puede generar con el código siguiente:

```latex
$\int (2x^3 + 58x + 29)\text{d}x$
```

Para escribir ecuaciones, es necesario entrar a un modo llamado `mathmode`. Hay varias versiones de este modo, pero las más usadas son **inline** y **display**. La primera habla de ecuaciones *en la misma línea*, es decir, dentro del cuerpo del párrafo así como $\sum_{i=0}^{n=\infty}x^i$.
El otro modo, **display**, es para *mostrar* ecuaciones en una línea nueva, usualmente centrada; así:

$$ c^2 = \sqrt{a^2 + b^2} $$

Para entrar en **inline mode** usamos un signo de peso/dólar `$` antes y después de la ecuación (como en el ejemplo anterior). Entrar a **display mode** es similar, pero usando dos signos de peso/dólar `$$`. De manera alternativa, puedes utilizar `\( inline eq \)` y `\[ display eq. \]` para delimitar el inicio y el fin de **inline** y **display mode** respectivamente.

Para ver más ejemplos, puedes hacer clic derecho sobre las ecuaciones de esta página y revisar los comandos utilizados para crearlas, bajo el apartado *Show Math As* > *TeX Commands*.

## Comentarios finales

Todo esto suena a ser sólo la punta de un iceberg monstruoso, pero la verdad es que vale la pena.
Sin embargo, no es sencillo empezar, así que no recomiendo que te aventures a intentarlo un día antes de la entrega de una tarea.
Considera si puedes y quieres dedicarle unas cuántas noches a aprender a usar LaTeX. Si es así, practica y estoy seguro de que podrás encontrarle mucha utilidad.

Si tienes más dudas, puedes preguntar aquí o enviarme un correo.