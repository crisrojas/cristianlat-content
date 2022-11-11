
### Zettels

El hermano mayor de _MiyanoSwift_. Empecé con este proyecto antes de usar _Bear_.

En esa época tomaba notas en formato de texto con aplicaciones como _The Archive_, _Obsidian_, _Notable_, etc...

Quería publicar mis notas para crear lo que algunos llaman _"Jardín digital"_ o _"Digital Garden"_.

Utilicé _Hugo_. En esa época todavía no era programador profesional. Algunas de las funcionalidades me costaron bastante (los _wikilinks_, los _backlinks_, la barra de búsqueda, etc...)

<!-- @todo añadir primera versión del proyecto y changelogs-->

Después empecé a usar Bear y me obsesioné con la idea de publicar mis notas. Pero el proceso de exportar las notas de forma manual en Bear para dárselas a Hugo y transformarlas con Zettels no era una opción.

Investigué y encontré un pequeño script PHP en Github creado por Steve Francia[^sfrancia] en Github con el que publicaba sus notas y me sirvió de base para crear un primer prototipo.

[^sfrancia]: Co-fundador de Panic

El principio era crear un repositorio en el que habría: la base de datos de Bear, el proyecto *Hugo* y el script PHP.

El repositorio era desplegado a _Netlify_, que estaba configurado para lanzar primero el script PHP (que exportaba las notas a la carpeta _content_ de _Hugo_) y luego el script de _Build_ de _Hugo_.

Al principio el proyecto convivía con mi blog personal (_cristian.lat_), pero me dí cuenta de la necesidad de separarlos en dos porque el repositorio se hacía cada vez más complejo ya quería que el blog tuviera un estilo diferente y cada vez que intentaba añadir algo al blog, rompía alguna cosa relacionada con las notas y viceversa.

Para ese entonces ya había empezado una carrera como desarrollador (aunque ~~seguía~~ sigo ~~muy~~ un poco verde) y pude sufrir en _"carne propia"_ los efectos de no aplicar la separación de responsabilidades [^concerns]

[^concerns]: _Separation of concerns_
