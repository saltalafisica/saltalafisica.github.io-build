# Donde van las cosas

El carrusel que esta en la primer pagina esta en la carpeta `data/carousel/*.yaml`.

La imagen de fondo del carrusel es la imagen `static/img/photogrid.png`.

Los logos `static/img/logo*`.

## Scripts utiles

### Agarra todas las imagenes en una carpeta y les da un tamaño de maximo 1200px y las optimiza para la web. se puede hacer mas ojo

```bash
magick mogrify -path output -resize 1200x\> -strip -interlace Plane -quality 82 *.jpeg
```

---

## TODO

- [x] Fix upper case troughot all of the text
- [x] Increase the width of the content column
- [x] RSS feed
- [x] Make giant tables scrollable
- [x] Fix translation issues in the table of contents (i38)
- [x] Ensure the banner image is displayed correctly
- [x] Other contribution channels
- [x] Document how to add a post and modify the site
- [ ] Get the new favicon
- [ ] Make the tag column toggable
- [ ] Display all affiliations
- [ ] Optimize images for the website
- [ ] Meta open graph optimization
- [ ] SEO optimization
- [ ] Setting the domain name
- [ ] Formulario de contacto
- [ ] Otras formas de apoyar a la asociacion. Con tiempo, contadores, cuestiones burocraticas y administrativas.

---

## Contribuciones

Aceptamos contribuciones a experimentos y todas son bienvenidas. Antes de considerarse un post definitivo debe seguir ciertos criterios.

Este checklist es una guía de estos criterios. Los posts deben contener:

- [ ] **Link a todos los recursos externos mencionados, imágenes, software, etc.** Por ejemplo, link a Phyphox, donde descargar software, etc.
- [ ] **Paso a paso del uso de herramientas externas si es que se usa.** Por ejemplo, capturas de la app Phyphox.
- [ ] **Donde conseguir material para experimentos.** Por ejemplo, donde comprar acetato.
- [ ] **Si es una traducción. Adaptar correctamente metadata, links, tags.**
- [ ] **Tratar de traducir los términos técnicos al español, pero incluyendo el término en inglés entre paréntesis.** Esto permite que sea fácil de googlear.
- [ ] **Redacción y ortografía.**

### Un template

Un template de post para este sitio:

```markdown
---
title: "Título del post"
author: Nombre de los autores separados por coma
subtitle: "📏➕📐" # tres emojis que tengan que ver con el post, podes sacarlos de https://emojipedia.org/
tags: [
    "Distancias",
    "Trigonometría",
    "Matemática",
    "Física",
    "Propagación de errores",
  ] # Por lo general contienen lo mismo que los temas
date: 2022-10-15 # poner la fecha de creación del post
math: true # si contiene ecuaciones poner true
image: false # a definir en el futuro que tipo de imagenes poner, por el momento queda false
---

Oración que aparecerá en el resúmen del post

<!--more-->

---

- **Dificultad:** ★★☆☆☆

- **Materiales:**
  - Material o recurso con su link
  - Otro
  - Tantos como haga falta

- **Duración de preparación:** 30 min

- **Temas:** Distancias, trigonometría, matemática, física, propagación de errores <!-- Los temas separados por comas. Por ej:  -->

---

Se pueden poner parrafos. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Se pueden poner imágenes así

![](/img/plano.webp)

Vale poner ecuaciones y se vuelven scrolleables si son muy largas:

$$
\tan (x), \int, \sum, \prod, \int, \sum, \prod, \int, \sum, \prod,
1, 2, 3, 4, 5, 6 \dots \infty,
\cos^2 \theta + \sin^2 \theta = 1
$$

También se pueden introducir en la misma línea \\( \tan(x) \\).

También se pueden poner matrices y estructuras similiares, pero se debe tener en cuenta que algunas expresiones de latex que tienen doble "\\". Pueden requerir triple "\\" por como se procesan las ecuaciones en nuestro template de hugo.

$$
\left \lbrace
    \begin{matrix}
    1 & 5 & 8 \\\
    0 & 2 & 4 \\\
    3 & 3 & -8
    \end{matrix}
\right \rbrace
$$

### Recomendado para aprender más

- [Absorción de luz (Hyperphysics)](http://hyperphysics.phy-astr.gsu.edu/hbasees/phyopt/absorb.html#c1)
- [Intensidad de luz (Hyperphysics)](http://hyperphysics.phy-astr.gsu.edu/hbasees/vision/photom.html#c1)
- Capítulo de un libro (Si aplica)
- Otro post en este sitio (Si aplica)
```
