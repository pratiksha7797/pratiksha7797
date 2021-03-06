---
title: Crear gists
intro: 'Puedes crear dos tipos de gists: {% ifversion ghae %}internos{% else %}públicos{% endif %} y secretos. Crea un gist {% ifversion ghae %}interno{% else %}público{% endif %} si estás listo para compartir tus ideas con {% ifversion ghae %}los miembros de la emrpesa{% else %}el mundo{% endif %} o, de lo contrario, un gist secreto.'
permissions: '{% data reusables.enterprise-accounts.emu-permission-gist %}'
redirect_from:
  - /articles/about-gists/
  - /articles/cannot-delete-an-anonymous-gist/
  - /articles/deleting-an-anonymous-gist/
  - /articles/creating-gists
  - /github/writing-on-github/creating-gists
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
---

## Acerca de los gists

Todo gist es un repositorio Git, lo que significa que se puede bifurcar y clonar. {% ifversion not ghae %}Si iniciaste sesión en {% data variables.product.product_name %} cuando{% else %}Cuando{% endif %} creas un gist, este se asociará con tu cuenta y lo verás en tu lista de gists cuando navegues a tu {% data variables.gists.gist_homepage %}.

Los gists pueden ser {% ifversion ghae %}internos{% else %}públicos{% endif %} o secretos. Los gists {% ifversion ghae %}internos{% else %}públicos{% endif %} se muestran en {% data variables.gists.discover_url %}, en donde {% ifversion ghae %}los miembros empresariales{% else %}las personas{% endif %} pueden buscar gists nuevos conforme estos se creen. También se los puede buscar, para que puedas usarlos si deseas que otras personas encuentren tu trabajo y lo vean.

Los gists secretos no se muestran en {% data variables.gists.discover_url %} y no se pueden buscar. Los gists no son privados. Si envías la URL de un gist secreto a {% ifversion ghae %}otro miembro de la empresa{% else %}un amigo {% endif %}, podrán verlo. Sin embargo, si {% ifversion ghae %}cualquier otro miembro de la empresa{% else %}alguien que no conozcas{% endif %} descubre la URL, también podrán ver tu gist. Si deseas mantener tu código a salvo de las miradas curiosas, puedes optar por [crear un repositorio privado](/articles/creating-a-new-repository) en lugar de un gist.

{% data reusables.gist.cannot-convert-public-gists-to-secret %}

{% ifversion ghes %}

Si el administrador de tu sitio ha inhabilitado el modo privado, también puedes usar gists anónimos, que pueden ser públicos o privados.

{% data reusables.gist.anonymous-gists-cannot-be-deleted %}

{% endif %}

Recibirás una notificación si:
- Seas el autor de un gist.
- Alguien te mencione en un gist.
- Puedes suscribirte a un gist haciendo clic en **Suscribir** en la parte superior de cualquier gist.

{% ifversion fpt or ghes %}

Puedes fijar los gists a tu perfil para que otras personas los puedan ver fácilmente. Para obtener más información, consulta "[A nclar elementos a tu perfil](/articles/pinning-items-to-your-profile)".

{% endif %}

Puedes descubrir gists {% ifversion ghae %}internos{% else %}públicos{% endif %} que hayan creado otras personas si vas a la {% data variables.gists.gist_homepage %} y das clic en **Todos los gists**. Esto te llevará a una página en la que aparecen todos los gists clasificados y presentados por fecha de creación o actualización. También puedes buscar los gists por idioma con {% data variables.gists.gist_search_url %}. La búsqueda de gists usa la misma sintaxis de búsqueda que la [búsqueda de código](/search-github/searching-on-github/searching-code).

Dado que los gists son repositorios Git, puedes ver su historial de confirmaciones completo, que incluye todas las diferencias que existan. También puedes bifurcar o clonar gists. Para obtener más información, consulta "[Bifurcar y clonar gists"](/articles/forking-and-cloning-gists).

Puedes descargar un archivo ZIP de un gist haciendo clic en el botón **Descargar ZIP** en la parte superior del gist. Puedes insertar un gist en cualquier campo de texto compatible con Javascript, como una publicación en un blog. Para insertar el código, haz clic en el icono del portapapeles junto a la URL **Insertar** de un gist. Para insertar un archivo de gist específico, anexa la URL **Insertar** con `?file=FILENAME`.

{% ifversion fpt %}

Git admite la asignación de archivos GeoJSON. Estas asignaciones se muestran como gists insertos, para que las asignaciones se puedan compartir e insertar fácilmente. Para obtener más información, consulta la sección "[Trabajar con archivos que no sean de código](/repositories/working-with-files/using-files/working-with-non-code-files#mapping-geojson-files-on-github)".

{% endif %}

## Crear un gist

Sigue estos pasos para crear un gist.

{% ifversion fpt or ghes or ghae %}
{% note %}

También puedes crear un gist si utilizas el {% data variables.product.prodname_cli %}. Para obtener más información, consulta "[`gh gist create`](https://cli.github.com/manual/gh_gist_create)" en el {% data variables.product.prodname_cli %}.

Como alternativa, puedes arrastrar y soltar un archivo de texto desde tu escritorio directamente en el editor.

{% endnote %}
{% endif %}

1. Inicia sesión en {% data variables.product.product_name %}.
2. Dirígete a tu {% data variables.gists.gist_homepage %}.
3. Escribe una descripción opcional y un nombre para tu gist. ![Descripción del nombre del gist](/assets/images/help/gist/gist_name_description.png)

4. Teclea el texto de tu gist en la caja de texto de este. ![Cuadro de texto para el gist](/assets/images/help/gist/gist_text_box.png)

5. Opcionalmente, para crear un gist {% ifversion ghae %}interno{% else %}público{% endif %}, da clic en {% octicon "triangle-down" aria-label="The downwards triangle icon" %} y luego en **Crear gist {% ifversion ghae %}interno{% else %}público{% endif %}**. ![Menú desplegable para seleccionar la visibilidad de un gist]{% ifversion ghae %}(/assets/images/help/gist/gist-visibility-drop-down-ae.png){% else %}(/assets/images/help/gist/gist-visibility-drop-down.png){% endif %}

6. Da clic en **Crear Gist Secreto** o en **Crear gist {% ifversion ghae %}interno{% else %}público{% endif %}**. ![Botón para crear gist](/assets/images/help/gist/create-secret-gist-button.png)
