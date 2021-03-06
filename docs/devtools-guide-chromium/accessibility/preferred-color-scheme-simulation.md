---
description: Force Microsoft Edge DevTools into Color Scheme Preview mode.
title: Force Microsoft Edge DevTools into Color Scheme Preview mode (CSS Prefers Color Scheme)
author: MSEdgeTeam
ms.author: msedgedevrel
ms.date: 02/12/2021
ms.topic: article
ms.prod: microsoft-edge
keywords: microsoft edge, web development, f12 tools, devtools
---

Operating systems have a way to display any application in darker or lighter colors.  Having a web product that has a light theme in a dark mode operating system is grating and can be an accessibility issue for some users.  On the web, you may use the [prefers-color-scheme][MDNPrefersColorScheme] CSS Media Query to detect if users prefer to display your product in a darker or lighter colour scheme.  Use [Microsoft Edge DevTools][DevtoolsIndex] to simulate a change from dark to light mode without having to change the entire operating system.

1.  Open the **Command Menu**.
    1.  Select `Ctrl`+`Shift`+`P` \(Windows/Linux\) or `Command`+`Shift`+`P` \(macOS\).

        :::image type="complex" source="../media/css-console-command-menu-rendering.msft.png" alt-text="The Command Menu" lightbox="../media/css-console-command-menu-rendering.msft.png":::
           The **Command Menu**
        :::image-end:::

1.  Type `emulate color`, choose either **Emulate CSS prefers-color-scheme: dark** or **Emulate CSS prefers-color-scheme: light** and then select `Enter`.

    :::image type="complex" source="../media/css-elements-styles-qs-select-renderingmode-command-menu.msft.png" alt-text="Color scheme option from Command Menu" lightbox="../media/css-elements-styles-qs-select-renderingmode-command-menu.msft.png":::
       Color scheme option from **Command** Menu
    :::image-end:::

    > [!IMPORTANT]
    > Simply typing `dark` or `light` does not reveal the right tool, since there is also a way to [choose a theme for DevTools][DevtoolsCustomizeDarkTheme].  If you are wondering what to choose, make sure that you are choosing a **rendering** menu item, not an **appearance** menu item.

1.  After you choose a color scheme, refresh the current document to display the simulated mode.

    :::image type="complex" source="../media/css-elements-styles-qs-simulated-light-mode.msft.png" alt-text="Simulated light mode inside Microsoft Edge DevTools" lightbox="../media/css-elements-styles-qs-simulated-light-mode.msft.png":::
       Simulated light mode inside Microsoft Edge DevTools
    :::image-end:::

    View and change your CSS like any other web page.  For more information, navigate to [Get Started With Viewing And Changing CSS][DevtoolsCssIndex].

<!-- links -->

[DevtoolsIndex]: ../index.md "Microsoft Edge (Chromium) Developer Tools | Microsoft Docs"
[DevtoolsCustomizeDarkTheme]: ../customize/dark-theme.md "Enable Dark Theme In Microsoft Edge DevTools | Microsoft Docs"
[DevtoolsCssIndex]: ../css/index.md "Get Started With Viewing And Changing CSS | Microsoft Docs"

[MDNPrefersColorScheme]: https://developer.mozilla.org/docs/Web/CSS/@media/prefers-color-scheme "prefers-color-scheme | MDN"
<link rel="stylesheet" href="//axeleric.eu/assets/md/css/ae-md.css">
<link rel="stylesheet" href="//axeleric.eu/assets/md/css/ae-md-append.css">
<link rel="stylesheet" href="//axeleric.eu/assets/md/css/ae-md-col3.css">
<link rel="stylesheet" href="//axeleric.eu/assets/md/css/ae-hili.css">
<script src="//axeleric.eu/assets/md/js/highlight.pack.js"></script>
<script>hljs.highlightAll();</script>

<div id="left-box" class="left-box">

**Table Of Content**

</div>

<div id="right-box" class="right-box">

[**In This Article**](#top)

</div>

<div id="top-box" class="top-box">&nbsp;

# Dark or Light Color Scheme simulation  


</div>
