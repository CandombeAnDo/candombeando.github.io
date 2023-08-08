## Tipos de página


Cuatro tipos de página:

- **homepage** [&rarr;](#homepage)
- **info-about** [&rarr;](#info-about)
- **listado de sección**[&rarr;](#listado-de-sección)
- **página con ítem**[&rarr;](#página-con-ítem)

### homepage

Página de inicio del sitio (primer nivel), con presentación general y un carrusel de imágenes/videos con links a las secciones importantes: registros, publicaciones, recursos, etc.

También puede tener un recuadro con novedades/noticias.

### info-about

Páginas de segundo nivel, con información y que no tienen un sub-nivel asociado:

- introducción a candombe
- info del proyecto
- ...

### listado de sección

Páginas de segundo nivel, con listado de todos [ítems](#página-con-ítem) pertenecientes a una categoría. Las listas son generadas automáticamente por Hugo.


### página con ítem

Páginas del nivel más bajo, con la información detallada de un/a: 

- publicación
- registro
- proyecto
- recurso
- evento (sesión de registros, presentación en congreso, conferencias, ...??)
- integrante
- ...

Cada una de estas categorías va a tener un `archetype`, (e.g [`pubs.md`](../archetypes/pubs.md)), con los campos específicos.

Los estilos y el formato de cada tipo de página va a tener que ajustarse en función de los campos específicos.


---


## Estructura de página

```
 _______________________________________________________________________
| _____________________________NAVBAR__________________________________ |
||                   ||                                                ||
||       LOGO        ||                     MENU                       ||
||___________________||________________________________________________||
|_______________________________________________________________________|
 _______________________________________________________________________
|                                                                       |
|                                                                       |
|                              HEADER                                   |
|                                                                       |
|_______________________________________________________________________|
 _______________________________________________________________________
|                                                                       |
|                                                                       |
|                                                                       |
|                                                                       |
|                                                                       |
|                                                                       |
|                                                                       |
|                                                                       |
|                                                                       |
|                             ( CONTENT )                               |
|                                                                       |
|                                                                       |
|                                                                       |
|                                                                       |
|                                                                       |
|                                                                       |
|                                                                       |
|                                                                       |
|                                                                       |
|_______________________________________________________________________|
 _______________________________________________________________________
|                                                                       |
|                               FOOTER                                  |
|_______________________________________________________________________|

```

### navbar --- footer

Común a todas las páginas del sitio. El `navbar` tiene el logo y el menú, y el `footer` puede tener información de copyright y contacto.

- [navbar.html](../themes/aucd/layouts/partials/navbar.html)  
- [footer.html](../themes/aucd/layouts/partials/footer.html)


### head

Pueden ser de tres tipos:

- homepage
- sección
- página

### content

Depende del [tipo](#tipos-de-página) (y subtipo) de página.



---


## Menú

**About**

- Introducción al candombe
- Info del proyecto
- Equipo

(Páginas tipo [info-about](#info-about))

**Investigación**

- Proyectos
- Publicaciones

(Páginas tipo [listado de sección](#listado-de-sección))

**Recursos**

- Registros
- Transcripciones
- Software
- Colecciones

(Páginas tipo [listado de sección](#listado-de-sección))

**Eventos**

- Presentaciones en congresos
- Presentaciones en workshops, coloquios, etc
- Conferencias
- Sesión de registros
- Actividades de extensión (Casa de la Cultura, EP en la EUM)
- ...

(Página tipo [listado de sección](#listado-de-sección))
