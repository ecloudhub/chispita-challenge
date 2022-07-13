# Chispita Frontend Challenge

El desafío es armar una homepage para Nomad, una cadena de hoteles para trabajadores nómades (como muchos de nosotros 🧳)

## Instrucciones generales:
- [El diseño](https://www.figma.com/file/3i8cpMAejvHgRdsaFGaFHj/Chispa-Challenge-Nomad) está subido a Figma, la app que usamos para todos nuestros proyectos
- Armamos varios niveles de complejidad:
  - El main es el único obligatorio
  - De los sides tenés que hacer al menos uno, pero mientras más hagas obvio que mejor!
- Stack tecnológico 🤖:
  - `Next.js` cargando la información del lado del servidor para mejorar el SEO de la página
  - Para CSS + componentes usamos `Chakra-UI` pero sentite libre de usar lo que quieras!
  - Para fetchear data nos gusta usar React Query y Axios, pero lo dejamos a tu criterio
  - Preferimos Typescript 🤟
  - Podés usar cualquier librería extra con la que te sientas cómodo
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
- Crear una API utilizando el router que provee Next.js, que devuelva la data que consume la página. Endpoints:
  - `/api/nav`: devuelve un array con los links para el nav
  - `/api/footer`: devuelve la data para el footer
  - `/api/home`: devuelve la data para los componentes generales de la home
  - `/api/hotels/availability`: devuelve el listado de hoteles con información sobre disponibilidad para utilizar en el drawer
- Llamar a los endpoints de contenido para poder renderizar la home desde el servidor
- Llamar al endpoint de disponibilidad solo cuando se abra el drawer de reserva

### Sidequest 1
- Maquetar el diseño para celulares con la metodología mobile first (recomiendación: si elegís hacer esto, planealo desde el principio 😉)

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
- Nos acordamos tarde de que los hoteles reciben tráfico de todo el mundo 👽. Agregarle funcionalidad al botón `English` del nav, haciendo que todo el sitio se traduzca al inglés (Goole Translate FTW)

Happy coding! 👾
