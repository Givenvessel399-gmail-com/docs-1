---
title: Working collaboratively in a codespace
shortTitle: Work collaboratively
intro: 'You can work collaboratively with other people in a codespace by using {% data variables.product.prodname_vs %} Live Share.'
versions:
  fpt: '*'
  ghec: '*'
type: how_to
topics:
  - Codespaces
  - Developer
---

{% data variables.product.prodname_vs %} Live Share lets you collaboratively edit and debug with others in real time, within a codespace. You can securely share your current codespace, or access a codespace created by someone else.

You can start a Live Share session either within the {% data variables.product.prodname_vscode_shortname %} web client in your browser, or within the {% data variables.product.prodname_vscode_shortname %} desktop application.

For more information about Live Share, see "[What is {% data variables.product.prodname_vs %} Live Share?](https://learn.microsoft.com/en-us/visualstudio/liveshare/)" in the {% data variables.product.prodname_vs %} documentation.

## Sharing your codespace with someone else

1. In the Activity Bar, click the Extensions icon.
1. In the search box, type `Live Share`.

   ![Screenshot of searching for the Live Share extension](/assets/images/help/codespaces/live-share-search-extensions.png)

1. If the **Install** button is displayed beside the extension, click it to install the extension in the codespace.
1. If the extension is shown grayed out in the list, right-click it and click **Enable**.

   ![Screenshot of the 'Enable' right-click menu option](/assets/images/help/codespaces/live-share-enable-rightclick.png)

1. In the Activity Bar, click the Live Share icon.

   ![Screenshot of clicking the Live Share icon](/assets/images/help/codespaces/live-share-click-icon.png)

1. Click **Share**.

   ![Screenshot of the 'Share' button](/assets/images/help/codespaces/live-share-click-share.png)

   A "toast" notification message is displayed at the bottom right corner of {% data variables.product.prodname_vscode_shortname %}, telling you that a link to your codespace has been copied to the clipboard. You can click **Make read-only** if you want to prevent guests from making changes to the files you share with them.

   ![Screenshot of the Live Share session 'toast' message](/assets/images/help/codespaces/live-share-link-copied-clipboard.png)

1. Send the link in your clipboard to anyone you want to join you in your Live Share session.

   {% note %}

   **Important**: Given the level of access Live Share sessions can provide to guests, you should only share with people you trust, and you should think through the implications of what you are sharing. For more information, see "[Security features of Live Share](https://learn.microsoft.com/en-us/visualstudio/liveshare/reference/security)" in the {% data variables.product.prodname_vs %} documentation.

   {% endnote %}

## Stopping a Live Share session

To stop sharing your codespace, click the stop icon in the Live Share panel.

![Screenshot of the stop icon in the Live Share panel](/assets/images/help/codespaces/live-share-stop-collaboration.png)

If you, as the person who started the Live Share session, close the codespace the sharing session ends, even if the codespace remains active on the remote host.

The idle timeout, which automatically stops a codespace after a period of inactivity, only applies to the person who started the codespace. It does not apply to people who are working on the codespace via Live Share. The codespace may therefore time out while collaborators are using the codespace if the person who started the codespace remains inactive for the configured period of time. For more information, see "[Setting your timeout period for GitHub Codespaces](/codespaces/customizing-your-codespace/setting-your-timeout-period-for-github-codespaces)."

## Working collaboratively in someone else's codespace

If you want to work with someone within a codespace they've created, ask them to set up a Live Share session and send you a link, as described above.
