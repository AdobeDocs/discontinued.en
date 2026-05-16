---
title: Hidden test
description: This is a hidden test
hide: true
landing-page-breadcrumb-title: Test AEM 6.5
landing-page-name: experience-manager-65
feature: Annotations
exl-id: e6e5ba1c-98a5-4d7d-9913-426df31bc7a3
---
# Hidden test

May 15

Testing new key

This is a hidden test. I'm adding this `[` to make sure it works ok in v2 rendering!

## Open in new tab {#section_92882928}

`[See What's new](auditor.md) {target="_blank"}`

[Open in same tab](auditor.md)

[New tab with space with quotes](auditor.md) {target="_blank"}

[New tab with Anchor](auditor.md){target="_blank}

[New tab without space with quotes](auditor.md){target="_blank"}

[New tab with space without quotes](auditor.md) {target=_blank}

[New tab without space without quotes](auditor.md){target=_blank}

[New tab with deep link](commerce-channels.md#channel-manager-extension){target="_blank"}

[Anchor New tab with deep link](https://experienceleague.adobe.com/en/docs/analytics/analyze/home#key-analytics-resources){target="_blank"}

[New tab with external link](https://www.adobe.com){target="_blank"}

[New tab root link](/help/guide-1/auditor.md){target="_blank"}


<table>
  <tr>
    <th>With quotes</a></th>
    <th>Without quotes</th>
  </tr>
  <tr>
    <td><a href="https://www.adobe.com" target="_blank">Adobe new tab</a></td>
    <td><a href="https://www.adobe.com" target=_blank>Adobe new tab</td>
  </tr>
  <tr>
    <td><a href="https://www.adobe.com">Adobe no new tab</a></td>
    <td><a href="https://www.adobe.com">Adobe no new tab</td>
  </tr>
</table>

## Comment test

November 18, 2025

<!-- 
## Comment with basic text

This is a new line.

Second new line. 
-->


Comment below. If this is the last thing you see in this article, it's due to the comment syntax.

1. Click **[!UICONTROL Create]**.

<!-- 
## Create an exclusion using Advanced Search

You can also create exclusions using [!UICONTROL Advanced Search] on the [Catalog Search](/help/main/c-recommendations/c-products/catalog-search.md#save-as) page ( [!UICONTROL Recommendations] > [!UICONTROL Catalog Search] > [!UICONTROL Advanced Search]). 

![Save as dialog](/help/main/c-recommendations/c-products/assets/save-as.png)

After creating a search using "id > contains," for example, you can then click [!UICONTROL Save As] > [!UICONTROL Exclusion].

>[!IMPORTANT]
>
>The [!UICONTROL Advanced Search] functionality is case-insensitive; however, products returned at the time of delivery are based on case-sensitive search. This mismatch might lead to confusion. Ensure that you consider case-sensitivity when you create exclusions based on results using the Advanced Search functionality. For example, if you perform a search for "Holiday," that initial search lists results containing "Holiday" and "holiday." If you then create an exclusion with the intent to exclude products containing "holiday," only products containing "holiday" are excluded. Products containing "Holiday" are not excluded. 
-->

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
