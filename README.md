# Práctica 5 — Inventario

Código de arranque de la Práctica 5 de TC2007B.

Es una app de inventario **terminada**: lista, detalle y formulario, con
navegación y validación. Puedes agregar, editar, vender y borrar productos.

Le falta una sola cosa, y es el tema de la práctica: los datos viven en una
lista en memoria. Agrega un producto, cierra la app desde el selector de
aplicaciones y vuelve a abrirla — no está.

## Cómo empezar

1. Clona el repositorio y ábrelo en Android Studio.
2. Espera a que Gradle sincronice y corre la app: debes ver tres productos.
3. Comprueba el bug de arriba antes de leer nada más.
4. Sigue la guía: https://startdroid.com/practicas/inventario.html

## Cómo trabajar

Haz un commit en cada checkpoint de la guía:

    git add -A ; git commit -m "checkpoint a1"

Si algo se rompe sin remedio, `git restore .` te regresa al último checkpoint bueno.

Los experimentos que rompen el código a propósito van en una rama:

    git switch -c experimento-d3                  # antes de romper nada
    git add -A ; git commit -m "experimento-d3"   # al terminar: guárdalo EN la rama
    git switch main                               # el código bueno vuelve intacto

Sin el commit en la rama, `git switch main` se lleva tus cambios contigo y
el código roto aparece en `main`.

## Uso de IA

Todo commit con código generado por IA debe declararlo con un trailer
`Co-Authored-By`. Ver la política completa en la guía.

## Entrega

Ver la rúbrica en la guía. Al subir tu repositorio, sube también la rama del
experimento: `gh repo create … --push` solo sube la rama actual.

    git push origin --all
