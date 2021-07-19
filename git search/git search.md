# Git search

## Git grep

Git tiene herramientas para ayudarnos a buscar a traves de los directorios y archivos.
La utilidad es ```git grep```.

Para trabajar esta utilidad se utilizará el código fuente de DOOM.

Por ejemplo, queremos buscar un dialogo

> You're trying to say you like DOS better than me, right?

```git grep -i DOS```

Utilizamos el flag -i para indicar que no distingue entre mayusculas y minusculas.

Seguimos en la búsqueda del dialogo

```git grep -i "DOS better```

Para acotar más la búsqueda podemos utilizar regex (Regular expressions).

```git grep -i "DOS.*better```

Ademas podemos identificar en que linea se encuentra con ```-n``` o ```--line-number```

```git grep -n "You got the BFG9000!"```

Existen mas opciones dentro de la utilidad git grep. Para mas informacion https://git-scm.com/docs/git-grep.
