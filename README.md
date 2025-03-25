# Ecloud Frontend Challenge

El desafío es armar una homepage para Nomad, una cadena de hoteles para trabajadores nómades (como muchos de nosotros 🧳)

## Instrucciones generales:
- [El diseño](https://www.figma.com/design/y06rSLImOcbTmEbmbriZfY/Frontend---Challenge) está subido a Figma. A veces es más cómodo tener permisos de edición para tener un mayor control sobre el board, para esto recomendamos copiarse todo el contenido y pegarlo en uno nuevo 🙃.
- Armamos varios niveles de complejidad:
  - El main es el único obligatorio
  - De los sides tenés que hacer al menos uno, pero mientras más hagas obvio que mejor!
- Stack tecnológico 🤖:
  - `Next.js` con `App Router` cargando la información del lado del servidor para mejorar el SEO de la página
  - Para CSS y componentes usamos `Chakra-UI v3`, pero sentite libre de usar lo que quieras!
  - Preferimos Typescript 🤟
  - Podés usar cualquier librería extra con la que te sientas cómodo
- Necesitamos que subas el resultado a vercel y nos des el link
- No te olvides de subirlo a Github

### Main Story
- Maquetar el diseño desktop:
  - Nav con dropdown al hacer hover en `Experimenta`
  - Hero estático, sin slider
  - Drawer de la derecha al hacer click en `Reservar` del Nav
  - Frase ocupando al menos el 100% de la pantalla
  - Listado de hoteles:
    - Al hacer hover sobre un hotel se le aplica un blur a la caja y se expande la descripción
    - Utilizar alguna librería de slider. Tener cuidado de que al llegar al último slide quede alineado con el contenedor
  - Footer
- Llamar a los endpoints de contenido para poder renderizar la home desde el servidor
- Llamar al endpoint de disponibilidad solo cuando se abra el drawer de reserva

### Sidequest 1
- Maquetar el diseño para celulares con la metodología mobile first (recomendación: si elegís hacer esto, planealo desde el principio 😉)

### Sidequest 2
- Al equipo de UX/UI se olvidó de agregar los estilos para los hovers de los componentes 🙄. Usando tu propio criterio, sumale estilos y transiciones a los elementos que consideres deberían tenerlos
- Hacer que el nav se oculte al scrollear hacia abajo, y que vuelva a aparecer al scrollear hacia arriba

### Sidequest 3
- Agregar slider de imágenes al hero 🎠. Comportamiento:
  - Las imágenes se mueven horizontalmente de forma automática
  - El paginador debe funcionar al hacer click
  - Mostrar la página activa con una pequeña de barra de carga que crece hasta cambiar a la siguiente página

### Sidequest 4
- El cliente vio que la página del hotel de la competencia tiene un cursor que sigue al mouse a todas partes. Agregar un cursor circular que siga al mouse y tenga el siguiente comportamiento:
  - Al posicionarse sobre un link cualquiera debe agrandar su tamaño
  - Al posicionarse sobre el botón Reservar del nav debe transformarse en una carita sonriente 😍

### Sidequest 5
- Utiliza `Sanity` como herramienta de CMS para administrar y gestionar los contenidos del sitio.

### Sidequest Extra
- Nos acordamos tarde de que los hoteles reciben tráfico de todo el mundo 👽. Si hiciste el sidequest anterior, agrega la posibilidad al sitio de que tenga internationalization para inglés y español y que se pueda gestionar los contenidos desde el CMS.

**Happy coding!** 👾

> Dudas? Sentite libre de escribirnos.
