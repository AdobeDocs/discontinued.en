---
title: Hidden test
description: This is a hidden test
hide: true
hidefromtoc: true
landing-page-breadcrumb-title: Test AEM 6.5
landing-page-name: experience-manager-65
feature: Annotations
exl-id: e6e5ba1c-98a5-4d7d-9913-426df31bc7a3
---
# Hidden test

This is a hidden test. I'm adding this `[` to make sure it works ok in v2 rendering.

November 18, 2025

Comment below. If this is the last thing you see in this article, it's due to the comment syntax.

<!-- ### Comment syntax

This is a new section.

The comment syntax close is at the end of the line. -->

This line is after the comment.

## Video test

### Plain video no transcript - should show transcript because metadata.md trickle down

>[!VIDEO](https://video.tv.adobe.com/v/332116?hidetitle=true)

### With transcript set to true

>[!VIDEO](https://video.tv.adobe.com/v/332116?hidetitle=true){transcript=true}

### With transcript set to false - video transcript should not show

>[!VIDEO](https://video.tv.adobe.com/v/332116?hidetitle=true){transcript=false}

## Relative links

* [Overview](overview.md)
* [Search and promote](search-promote.md)
* [Social](social.md)

## Explicit deep link

[overview additional (root)](/help/guide-1/overview.md#additional-products)

[overview additional](overview.md#additional-products)

## Hover text test {#this-is-a-heading-anchor}

No hover text

```
![alt text](assets/maui-flip.jpg)
```

![alt text](assets/maui-flip.jpg)


Yes hover text

```
![alt text](assets/maui-flip.jpg "Hover text")
```

![alt text](assets/maui-flip.jpg "Hover text")

## Slide

Syntax:

```
>[!SLIDE](analyze-project)
https://experienceleague-stage.adobe.com/en/slides/analyze-project
```

Rendered:

<!--
>[!SLIDE](analyze-project)
-->

Bob: Remove the slide comment once you test the topic loc thing.

