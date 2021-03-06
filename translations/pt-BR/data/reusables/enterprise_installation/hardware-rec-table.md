{% ifversion ghes = 2.22 %}

{% note %}

**Nota**: Se você se juntou ao beta para {% data variables.product.prodname_actions %} ou {% data variables.product.prodname_registry %} e habilitou as funcionalidades, a sua instância irá exigir recursos adicionais de hardware. Os requisitos mínimos para uma instância com recursos beta habilitados estão em **negrito** na tabela a seguir. Para obter mais informações, consulte "[Recursos Beta em {% data variables.product.prodname_ghe_server %} 2.22](#beta-features-in-github-enterprise-server-222)".

{% endnote %}
{% endif %}

{% ifversion ghes > 2.22 %}
| Licenças de usuário                      | vCPUs | Memória | Armazenamento anexado | Armazenamento raiz |
|:---------------------------------------- | -----:| -------:| ---------------------:| ------------------:|
| Teste, demonstração ou 10 usuários leves |     4 |   32 GB |                150 GB |             200 GB |
| 10-3000                                  |     8 |   48 GB |                300 GB |             200 GB |
| 3000-5000                                |    12 |   64 GB |                500 GB |             200 GB |
| 5000-8000                                |    16 |   96 GB |                750 GB |             200 GB |
| 8000-10000+                              |    20 |  160 GB |               1000 GB |             200 GB |

{% else %}

| Licenças de usuário                      |                                                                                                          vCPUs |                                                                                                                Memória |                                                                                                  Armazenamento anexado | Armazenamento raiz |
|:---------------------------------------- | --------------------------------------------------------------------------------------------------------------:| ----------------------------------------------------------------------------------------------------------------------:| ----------------------------------------------------------------------------------------------------------------------:| ------------------:|
| Teste, demonstração ou 10 usuários leves |   2{% ifversion ghes = 2.22 %}<br/>ou [**4**](#beta-features-in-github-enterprise-server-222){% endif %} |   16 GB{% ifversion ghes = 2.22 %}<br/>ou [**32 GB**](#beta-features-in-github-enterprise-server-222){% endif %} | 100 GB{% ifversion ghes = 2.22 %}<br/>ou [**150 GB**](#beta-features-in-github-enterprise-server-222){% endif %} |             200 GB |
| 10-3000                                  |   4{% ifversion ghes = 2.22 %}<br/>ou [**8**](#beta-features-in-github-enterprise-server-222){% endif %} |   32 GB{% ifversion ghes = 2.22 %}<br/>ou [**48 GB**](#beta-features-in-github-enterprise-server-222){% endif %} | 250 GB{% ifversion ghes = 2.22 %}<br/>ou [**300 GB**](#beta-features-in-github-enterprise-server-222){% endif %} |             200 GB |
| 3000-5000                                |  8{% ifversion ghes = 2.22 %}<br/>ou [**12**](#beta-features-in-github-enterprise-server-222){% endif %} |                                                                                                                  64 GB |                                                                                                                 500 GB |             200 GB |
| 5000-8000                                | 12{% ifversion ghes = 2.22 %}<br/>ou [**16**](#beta-features-in-github-enterprise-server-222){% endif %} |                                                                                                                  96 GB |                                                                                                                 750 GB |             200 GB |
| 8000-10000+                              | 16{% ifversion ghes = 2.22 %}<br/>ou [**20**](#beta-features-in-github-enterprise-server-222){% endif %} | 128 GB{% ifversion ghes = 2.22 %}<br/>ou [**160 GB**](#beta-features-in-github-enterprise-server-222){% endif %} |                                                                                                                1000 GB |             200 GB |

{% endif %}

{% ifversion ghes > 2.22 %}

Se você planeja habilitar {% data variables.product.prodname_actions %} para os usuários da sua instância, verifique os requisitos para hardware, armazenamento externo e executores em "[Primeiros passos com {% data variables.product.prodname_actions %} para {% data variables.product.prodname_ghe_server %}](/admin/github-actions/getting-started-with-github-actions-for-github-enterprise-server)".

{% endif %}

{% data reusables.enterprise_installation.about-adjusting-resources %}

{% ifversion ghes = 2.22 %}

### Recursos do beta em {% data variables.product.prodname_ghe_server %} 2.22

{% data variables.product.prodname_ghe_server %} 2.22 ofereceu funcionalidades em beta, como {% data variables.product.prodname_actions %}, {% data variables.product.prodname_registry %} e {% data variables.product.prodname_code_scanning %}. Para obter mais informações, consulte as observações sobre a versão [{% data variables.product.prodname_ghe_server %} 2.22](/enterprise-server@2.22/admin/release-notes#2.22.0).

Se você habilitou funcionalidades em beta para {% data variables.product.prodname_ghe_server %} 2.22, sua instância irá exigir recursos adicionais de hardware. Para obter mais informações sobre requisitos mínimos, consulte "[Requisitos mínimos](#minimum-requirements)".

Para obter mais informações sobre os requisitos de hardware para {% data variables.product.prodname_actions %}, consulte "[Introdução a {% data variables.product.prodname_actions %} para {% data variables.product.prodname_ghe_server %}](/admin/github-actions/getting-started-with-github-actions-for-github-enterprise-server#review-hardware-considerations)".

{% endif %}
