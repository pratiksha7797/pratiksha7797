---
title: Ver las ramas en tu repositorio
intro: 'Las ramas son centrales para la colaboración en {% data variables.product.product_name %}, y la mejor manera de verlas es en la pagina de ramas.'
redirect_from:
  - /articles/viewing-branches-in-your-repository
  - /github/administering-a-repository/viewing-branches-in-your-repository
  - /github/administering-a-repository/managing-branches-in-your-repository/viewing-branches-in-your-repository
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
topics:
  - Repositories
shortTitle: Ver ramas
---

{% data reusables.repositories.navigate-to-repo %}
{% data reusables.repositories.navigate-to-branches %}
3. Utiliza la navegación en la parte superior de la página para ver las listas de ramas específicas:
    - **Tus ramas**: En los repositorios a los cuales hayas subido código, la vista de **Tuyos** muestra todas las ramas que has subido, excluyendo la predeterminada, con las ramas más recientes primero.
    - **Ramas activas**: la vista **Active** (Activas) muestra todas las ramas a las que alguien ha confirmado dentro de los últimos tres meses, ordenadas de forma descendente desde las ramas con las confirmaciones más recientes.
    - **Ramas en espera**: la vista **Stale** (En espera) muestra todas las ramas en las que nadie ha confirmado durante los últimos tres meses, ordenadas de forma descendente desde las confirmaciones más antiguas. Utiliza esta lista para determinar [qué ramas eliminar](/articles/creating-and-deleting-branches-within-your-repository).
    - **Todas las ramas**: la vista **All** (Todas) muestra la rama por defecto, seguida por todas las otras ramas ordenadas de forma descendente desde las ramas con las confirmaciones más recientes.

4. Opcionalmente, utiliza el campo de búsqueda en la parte superior derecha. Este proporciona una búsqueda de sub-secuencias simple y que distingue entre mayúsculas y minusculas para el nombre de rama. Esta no es compatible con ninguna sintaxis de consulta adicional.

![La página de ramas para el repositorio Atom](/assets/images/help/branches/branches-overview-atom.png)

## Leer más

- "[Crear y eliminar ramas dentro de tu repositorio](/articles/creating-and-deleting-branches-within-your-repository/)"
- "[Eliminar ramas no utilizadas](/articles/deleting-unused-branches)"
