---
title: Forwarding ports in your codespace
intro: '{% data reusables.codespaces.about-port-forwarding %}'
product: '{% data reusables.gated-features.codespaces %}'
versions:
  fpt: '*'
redirect_from:
  - /github/developing-online-with-codespaces/forwarding-ports-in-your-codespace
type: how_to
topics:
  - Codespaces
  - Fundamentals
  - Developer
shortTitle: ポートの転送
---

 

## About forwarded ports

ポート転送を使用すると、Codespaces 内で実行されている TCP ポートにアクセスできます。 For example, if you're running a web application on port 4000, you can access the application from your browser to test and debug the application.

When an application running inside a codespace outputs a port to the console, {% data variables.product.prodname_codespaces %} detects the localhost URL pattern and automatically forwards the port. You can click on the URL in the terminal to open the port in a browser. たとえば、アプリケーションが `http://127.0.0.1:4000` または `http://localhost:4000` をコンソールに出力する場合、ログは出力をポート 4000 のクリック可能な URL に自動的に変換します。

![Automatic port forwarding](/assets/images/help/codespaces/automatic-port-forwarding.png)

ポートの手動転送、転送されたポートへのラベル付け、転送されたポートのパブリックへの共有、転送されたポートの codespace 設定への追加ができます。

## Forwarding a port

You can manually forward a port that wasn't forwarded automatically.

{% data reusables.codespaces.navigate-to-ports-tab %}
1. Under the list of ports, click **Add port**. ![Add port button](/assets/images/help/codespaces/add-port-button.png)
1. Type the port number or address, then press enter. ![Text box to type port button](/assets/images/help/codespaces/port-number-text-box.png)

## Labeling a port

You can label a port to make the port more easily identifiable in a list.

{% data reusables.codespaces.navigate-to-ports-tab %}
1. Hover over the port you want to label, then click the label icon. ![Label icon for port](/assets/images/help/codespaces/label-icon.png)
{% data reusables.codespaces.type-port-label %}

## Sharing a port

If you want to share a forwarded port with others, you need to make the port public. After you make a port public, anyone with the port's URL can view the running application without needing to authenticate.

{% data reusables.codespaces.navigate-to-ports-tab %}
1. Right click the port you want to share, then click **Make Public**. ![Option to make port public in right-click menu](/assets/images/help/codespaces/make-public-option.png)
1. To the right of the local address for the port, click the copy icon. ![Copy icon for port URL](/assets/images/help/codespaces/copy-icon-port-url.png)
1. Send the copied URL to the person you want to share the port with.

## Adding a port to the codespace configuration

You can add a forwarded port to the {% data variables.product.prodname_codespaces %} configuration for the repository, so the port will automatically be forwarded for all codespaces created from the repository. After you update the configuration, any previously created codespaces must be rebuilt for the change to apply. 詳しい情報については、「[プロジェクトの {% data variables.product.prodname_codespaces %} を設定する](/codespaces/setting-up-your-codespace/configuring-codespaces-for-your-project#applying-changes-to-your-configuration)」を参照してください。

`forwardPorts` プロパティで `.devcontainer.json` ファイルで転送ポートを手動で設定するか、codespace の [Ports] パネルを使用できます。

{% data reusables.codespaces.navigate-to-ports-tab %}
1. Right click the port you want to add to the codespace configuration, then click **Set Label and Update devcontainer.json**. ![Option to set label and add port to devcontainer.json in the right-click menu](/assets/images/help/codespaces/update-devcontainer-to-add-port-option.png)
{% data reusables.codespaces.type-port-label %}
