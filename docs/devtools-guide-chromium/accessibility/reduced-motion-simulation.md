---
description: Simulate reduced motion using developer tools.
title: Simulate reduced motion using developer tools (CSS Prefers Reduced Motion)
author: MSEdgeTeam
ms.author: msedgedevrel
ms.date: 02/12/2021
ms.topic: article
ms.prod: microsoft-edge
keywords: microsoft edge, web development, f12 tools, devtools
---

Animation in web products may be an accessibility problem.  Operating Systems deal with the problem by including an option to turn off animations to avoid user confusion and potential health related problems such as triggering seizures.  On the web, you may use the [prefers-reduced-motion][MDNPrefersReducedMotion] CSS Media Query to detect if users prefer to not run or display any animations.  In your product, you may wrap your animation code in a test to avoid animations showing up for the affected users.

```css
@media (prefers-reduced-motion: reduce) {
  /* in case the .header element has an animation, turn it off */
  .header {
    animation: none;
  }
}
```

Using the [Microsoft Edge DevTools][DevtoolsIndex], you may simulate this reduced motion setting without having to change your operating system.

1.  Open the **Command Menu**.
    1.  Select `Control`+`Shift`+`P` on Windows/Linux or `Command`+`Shift`+`P` on macOS.

        :::image type="complex" source="../media/css-console-command-menu-rendering.msft.png" alt-text="The Command Menu" lightbox="../media/css-console-command-menu-rendering.msft.png":::
           The **Command Menu**
        :::image-end:::

1.  Type `reduced`, to turn the simulation on and off.  Choose the option and select `Enter`.

    :::image type="complex" source="../media/css-elements-styles-qs-select-reduced-motion-command-menu.msft.png" alt-text="Turn on or off the prefers reduced motion setting from Command Menu" lightbox="../media/css-elements-styles-qs-select-reduced-motion-command-menu.msft.png":::
       Turn on or off the **prefers reduced motion** setting from **Command Menu**
    :::image-end:::

1.  Refresh the current page to test whether your animations are turned off or visible.

<!-- links -->

[DevtoolsIndex]: ../index.md "Microsoft Edge (Chromium) Developer Tools | Microsoft Docs"

[MDNPrefersReducedMotion]: https://developer.mozilla.org/docs/Web/CSS/@media/prefers-reduced-motion "prefers-reduced-motion | MDN"
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

# Reduced motion simulation  


</div>
