---
title: Organization 内でリポジトリの作成を制限する
intro: Organization のデータを保護するために、Organization 内でリポジトリを作成するための権限を設定できます。
redirect_from:
  - /articles/restricting-repository-creation-in-your-organization
  - /github/setting-up-and-managing-organizations-and-teams/restricting-repository-creation-in-your-organization
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
topics:
  - Organizations
  - Teams
shortTitle: リポジトリの作成の制限
---

メンバーが Organization でリポジトリを作成できるかどうかを選択できます。 If you allow members to create repositories, you can choose which types of repositories members can create.{% ifversion fpt %} To allow members to create private repositories only, your organization must use {% data variables.product.prodname_ghe_cloud %}.{% endif %} For more information, see "[About repositories](/repositories/creating-and-managing-repositories/about-repositories#about-repository-visibility)."

Organization のオーナーは、いつでもどんなタイプの Team でも作成できます。

{% ifversion fpt %}Enterprise オーナー{% else %}サイト管理者{% endif %}は、Organization のリポジトリ作成ポリシーで使用できるオプションを制限できます。 詳しい情報については、{% ifversion fpt %}"「[Enterprise アカウントでリポジトリ管理ポリシーを施行する](/github/setting-up-and-managing-your-enterprise/enforcing-repository-management-policies-in-your-enterprise-account)」{% else %}「[Enterprise でのリポジトリの作成を制限する](/admin/policies/enforcing-repository-management-policies-in-your-enterprise#setting-a-policy-for-repository-creation)」{% endif %} を参照してください。

{% warning %}

**警告**: この設定で制限されるのは、リポジトリを作成するときの可視性オプションだけです。後からリポジトリの可視性を変更する機能は制限されません。 詳しい情報については「[Organization 内でリポジトリの可視性の変更を制限する](/organizations/managing-organization-settings/restricting-repository-visibility-changes-in-your-organization)」を参照してください。

{% endwarning %}

{% data reusables.organizations.internal-repos-enterprise %}

{% data reusables.profile.access_org %}
{% data reusables.profile.org_settings %}
{% data reusables.organizations.member-privileges %}
5. [Repository creation] で、1 つ以上のオプションを選択します。 ![リポジトリ作成のオプション](/assets/images/help/organizations/repo-creation-perms-radio-buttons.png)
6. [**Save**] をクリックします。
