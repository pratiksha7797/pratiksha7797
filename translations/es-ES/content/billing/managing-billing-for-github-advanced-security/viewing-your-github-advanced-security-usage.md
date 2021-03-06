---
title: Visualizar tu uso de GitHub Advanced Security
intro: 'Puedes ver el uso de {% data variables.product.prodname_GH_advanced_security %} de tu empresa.'
permissions: 'Enterprise owners can view usage for {% data variables.product.prodname_GH_advanced_security %}.'
product: '{% data reusables.gated-features.ghas %}'
redirect_from:
  - /billing/managing-licensing-for-github-advanced-security/viewing-your-github-advanced-security-usage
  - /admin/advanced-security/viewing-your-github-advanced-security-usage
  - /github/setting-up-and-managing-billing-and-payments-on-github/managing-licensing-for-github-advanced-security/viewing-your-github-advanced-security-usage
  - /github/setting-up-and-managing-your-enterprise/managing-use-of-advanced-security-for-organizations-in-your-enterprise-account
  - /github/setting-up-and-managing-billing-and-payments-on-github/viewing-your-github-advanced-security-usage
versions:
  ghes: '>=3.1'
  fpt: '*'
type: how_to
topics:
  - Advanced Security
  - Enterprise
shortTitle: Visualizar el uso de la Seguridad Avanzada
---

## Acerca de las licencias para {% data variables.product.prodname_GH_advanced_security %}

{% data reusables.advanced-security.about-ghas-license-seats %} Para obtener más información, consulta "[Acerca de la facturación para {% data variables.product.prodname_GH_advanced_security %}](/billing/managing-billing-for-github-advanced-security/about-billing-for-github-advanced-security)".

## Visualizar el uso del licenciamiento de {% data variables.product.prodname_GH_advanced_security %} para tu cuenta empresarial

Puedes verificar cuántas plazas incluye tu licencia y cuántas de ellas se están utilizando.

{% ifversion fpt %}

{% data reusables.enterprise-accounts.access-enterprise %}
{% data reusables.enterprise-accounts.settings-tab %}
{% data reusables.enterprise-accounts.license-tab %}
   La sección de "{% data variables.product.prodname_GH_advanced_security %}" muestra los detalles del uso actual. ![{% data variables.product.prodname_GH_advanced_security %} in enterprise licensing settings](/assets/images/help/enterprises/enterprise-licensing-tab-ghas.png) Si te quedas sin plazas, la sección estará en rojo y mostrará "Límite excedido". Debes ya sea reducir tu uso de {% data variables.product.prodname_GH_advanced_security %} o comprar más plazas. Para obtener más información, consulta la sección "[Acerca de la facturación para el {% data variables.product.prodname_GH_advanced_security %}](/billing/managing-billing-for-github-advanced-security/about-billing-for-github-advanced-security#getting-the-most-out-of-github-advanced-security)". ![{% data variables.product.prodname_GH_advanced_security %} en los ajustes de licenciamiento de empresa mostrando "Límite excedido"](/assets/images/help/enterprises/enterprise-licensing-tab-ghas-no-seats.png)
4. Opcionalmente, para ver un resumen detallado del uso por organización, en la barra lateral izquierda, haz clic en **Facturación**. ![Billing tab in the enterprise account settings sidebar](/assets/images/help/business-accounts/settings-billing-tab.png) En la sección de "{% data variables.product.prodname_GH_advanced_security %}" puedes ver la cantidad de confirmantes y confirmantes únicos de cada organización. ![{% data variables.product.prodname_GH_advanced_security %} en la configuración de facturación empresarial](/assets/images/help/billing/ghas-orgs-list-enterprise-dotcom.png)
5. Opcionalmente, haz clic en el nombre de una organización que te pertenezca para mostrar la configuración de seguridad y análisis para la organización. ![Organización que te pertenece en la sección de {% data variables.product.prodname_GH_advanced_security %} de la configuración de facturación empresarial](/assets/images/help/billing/ghas-orgs-list-enterprise-click-org.png)
6. En la página de configuración de "Seguridad & análisis", desplázate hacia la sección de "repositorios de {% data variables.product.prodname_GH_advanced_security %}" para ver un resumen detallado del uso de este repositorio en esta organización. ![{% data variables.product.prodname_GH_advanced_security %} repositories section](/assets/images/help/enterprises/settings-security-analysis-ghas-repos-list.png) Para obtener más información, consulta la sección "[Administrar la configuración de seguridad y análisis de tu organización](/organizations/keeping-your-organization-secure/managing-security-and-analysis-settings-for-your-organization)".

{% elsif ghes %}

{% data reusables.enterprise-accounts.access-enterprise %}
{% data reusables.enterprise-accounts.settings-tab %}
{% data reusables.enterprise-accounts.license-tab %}
   La sección de "{% data variables.product.prodname_GH_advanced_security %}" muestra los detalles del uso actual. Puedes ver la cantidad total de plazas utilizadas, así como una tabla con la cantidad de confirmantes y confirmantes únicos para cada organización. ![Sección de {% data variables.product.prodname_GH_advanced_security %} de la licencia empresarial](/assets/images/help/billing/ghas-orgs-list-enterprise-ghes.png)
5. Opcionalmente, haz clic en el nombre de una organización que te pertenezca para mostrar la configuración de seguridad y análisis para la organización. ![Organización que te pertenece en la sección de {% data variables.product.prodname_GH_advanced_security %} de la configuración de facturación empresarial](/assets/images/help/billing/ghas-orgs-list-enterprise-click-org.png)
6. En la página de configuración de "Seguridad & análisis", desplázate hacia la sección de "repositorios de {% data variables.product.prodname_GH_advanced_security %}" para ver un resumen detallado del uso de este repositorio en esta organización. ![{% data variables.product.prodname_GH_advanced_security %} repositories section](/assets/images/help/enterprises/settings-security-analysis-ghas-repos-list.png) Para obtener más información, consulta la sección "[Administrar la configuración de seguridad y análisis de tu organización](/organizations/keeping-your-organization-secure/managing-security-and-analysis-settings-for-your-organization)".

{% endif %}
