---
title: Sobre a identidade e gestão de acesso para a sua empresa
shortTitle: Sobre identidade e gestão de acesso
intro: 'Você pode usar a autenticação incluída em {% ifversion ghes %}{% data variables.product.prodname_ghe_server %} ou escolher entre CAS, LDAP, ou SAML{% else %}o logon único SAML (SSO) e o Sistema de Administração de Identidade de Domínio Cruzado (SCIM){% endif %} para administrar o acesso centralizadamente{% ifversion fpt %}para que as organizações pertencentes à sua empresa em {% data variables.product.prodname_dotcom_the_website %}{% endif %}{% ifversion ghes or ghae %}a {% data variables.product.product_location %}{% endif %}.'
product: '{% data reusables.gated-features.saml-sso %}'
versions:
  ghae: '*'
type: overview
topics:
  - Accounts
  - Access management
  - Authentication
  - Enterprise
  - Identity
redirect_from:
  - /admin/authentication/about-identity-and-access-management-for-your-enterprise
---

## Sobre a identidade e gestão de acesso para a sua empresa

{% ifversion ghae %}

{% data reusables.saml.ae-uses-saml-sso %} {% data reusables.saml.ae-enable-saml-sso-during-bootstrapping %}

Após configurar o aplicativo para {% data variables.product.product_name %} no seu IdP, você poderá conceder acesso a {% data variables.product.product_location %}, atribuindo o aplicativo a usuários e grupos no seu IdP. Para obter mais informações sobre o SAML SSO para {% data variables.product.product_name %}, consulte "[Configurar o logon único SAML para a sua empresa](/admin/authentication/configuring-saml-single-sign-on-for-your-enterprise)".

{% data reusables.scim.after-you-configure-saml %} Para obter mais informações, consulte "[Configurar provisionamento do usuário para sua empresa](/admin/authentication/configuring-user-provisioning-for-your-enterprise)".

Para aprender como configurar tanto o provisionamento de autenticação quanto o usuário para {% data variables.product.product_location %} com seu IdP específico, consulte "[Configurar autenticação e provisionamento com o seu provedor de identidade](/admin/authentication/configuring-authentication-and-provisioning-with-your-identity-provider)".

{% endif %}

## Leia mais

- [Wiki de SAML](https://wiki.oasis-open.org/security) no site OASIS
- [Sistema para Gerenciamento de Identidade de entre Domínios: Protocolo (RFC 7644)](https://tools.ietf.org/html/rfc7644) no site do IETF
- [Restringir o tráfego de rede para a sua empresa](/admin/configuration/restricting-network-traffic-to-your-enterprise)
