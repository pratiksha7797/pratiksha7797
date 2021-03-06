{% warning %}

**Advertencia:**

- Si eliminas el acceso de una persona a un repositorio privado, todas sus bifurcaciones de ese repositorio privado se eliminarán. Los clones locales del repositorio privado se conservarán. Si se revoca el acceso de un equipo a un repositorio privado o se elimina un equipo con acceso a un repositorio privado, y los miembros del equipo no tienen acceso al repositorio a través de otro equipo, las bifurcaciones privadas del repositorio se eliminarán.{% ifversion ghes %}
- Cuando [LDAP Sync esté habilitado](/enterprise/{{ page.version }}/admin/guides/user-management/using-ldap/#enabling-ldap-sync), si eliminas a una persona de un repositorio, perderá acceso, pero sus bifurcaciones no se eliminarán. Si la persona se agrega a un equipo con acceso al repositorio original de la organización dentro de los tres meses, su acceso a las bifurcaciones se restaurarán de manera automática la próxima vez que ocurra una sincronización.{% endif %}
- Eres responsable de asegurar que las personas que perdieron el acceso a un repositorio borren cualquier información confidencial o propiedad intelectual.

- Las personas con permisos administrativos en un repositorio privado{% ifversion fpt or ghes or ghae %} o interno{% endif %} pueden dejar de permitir la bifurcación del mismo, y los propietarios de la organización pueden dejar de permitir la bifurcación de cualquier repositorio privado {% ifversion fpt or ghes or ghae %} o interno {% endif %} en una organización. Para obtener más información, consulta las secciones "[Administrar la política de bifurcación para tu organización](/organizations/managing-organization-settings/managing-the-forking-policy-for-your-organization)" y "[Administrar la política de bifurcación para tu repositorio](/github/administering-a-repository/managing-the-forking-policy-for-your-repository)".

{% endwarning %}
