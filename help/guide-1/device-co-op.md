---
keywords: adobe experience cloud;Adobe Experience Cloud;device co-op;Device Co-op;end-of-life
title: "[!DNL Device Co-op] end-of-life FAQ"
description: Learn about the end-of-life plans for the Device Co-op.
exl-id: 015ba95c-0c8d-415e-969c-b8670494de98
---
# [!DNL Device Co-op] end-of-life FAQ

This document provides answers to frequently asked questions about the [!DNL Adobe Experience Cloud Device Co-op] end-of-life (EOL) plan. When this plan goes into effect, Adobe will provide an advanced notice in the [Experience Cloud release notes](https://experienceleague.adobe.com/docs/release-notes/experience-cloud/current.html) and the [Priority Product Update](https://www.adobe.com/subscription/priority-product-update.html).

[!DNL Device Co-op] was a program that let participants work together to better identify consumers across digital touch points while ensuring the highest level of privacy and transparency.

## FAQ

The following is a list of answers to frequently asked questions about the [!DNL Device Co-op] EOL plan.

## Why is [!DNL Device Co-op] being deprecated?

The upcoming changes in the AdTech environment are expected to result in [!DNL Device Co-op] becoming an obsolete solution in the coming years. [!DNL Device Co-op] is comprised mostly of third-party cookies and [!DNL Google's] announcement that they will be blocking third-party cookies on [!DNL Google Chrome] by 2022 will diminish the effectiveness of [!DNL Device Co-op]. [!DNL Chrome] has ~65% of the browser market share and other major browsers have already implemented blocking of third-party cookies. Once [!DNL Chrome] blocks third-party cookies, the majority of third-party cookies will be blocked and [!DNL Device Co-op] will be rendered obsolete.

## Why is Adobe ending [!DNL Device Co-op] sign-ups now?

Sign-ups are ending to prevent risks of not meeting customer expectations due to the upcoming industry changes around third-party cookies. [!DNL Device Co-op] takes a few months to be prepared and another few months to extract value from the service. Any further sign-ups at this point could result in brands not experiencing the full value of [!DNL Device Co-op].

## On July 2022, Google announced the delay of third-party cookie deprecation on Chrome to 2024. Will this affect the [!DNL Device Co-op] EOL plans?

No, Adobe's [!DNL Device Co-op] EOL plans will continue to remain the same and will not be extended.

## Can new customers sign up?

Starting June 11, 2021, Adobe will no longer accept new sign-ups to [!DNL Device Co-op].

## Are existing contracts being renewed?

Starting June 11, 2021, Adobe will no longer renew [!DNL Device Co-op] contracts. If you wish to continue using [!DNL Device Co-op] services, you may continue to do so under the current license terms until the program ends.

## What is the exact end date of the [!DNL Device Co-op] program?

The [!DNL Device Co-op] program will end in 2022. The specific timing and date depends on when [!DNL Google] starts to block third-party cookies. The decommissioning work is expected to start in September 2022.

## Which applications will be affected by the Device Co-op end of life?

The following applications will be affected by the [!DNL Device Co-op] end of life procedures:

- [[!DNL Adobe Analytics]](https://experienceleague.adobe.com/docs/analytics.html?lang=en)
- [[!DNL Adobe Audience Manager]](https://experienceleague.adobe.com/docs/audience-manager/user-guide/overview/aam-overview.html?lang=en)
- [[!DNL Adobe Advertising]](https://experienceleague.adobe.com/docs/advertising.html?lang=en)
- [[!DNL Adobe Target]](https://experienceleague.adobe.com/docs/target/using/introduction/intro.html?lang=en)

## What options do I have as alternatives to [!DNL Device Co-op]?

### [!DNL Analytics]

You can use the [!DNL Analytics] [Cross-Device Analytics (CDA)](https://experienceleague.adobe.com/docs/analytics/components/cda/overview.html) feature as it supports both the Adobe Experience Platform Identity Service [Private Graph](https://experienceleague.adobe.com/docs/analytics/components/cda/device-graph.html?lang=en) and [Field-Based Stitching](https://experienceleague.adobe.com/docs/analytics/components/cda/field-based-stitching.html?lang=en).

### [!DNL Audience Manager]

[!DNL Audience Manager] maintains integrations with third-party device graph partners including [!DNL LiveRamp] and [!DNL Tapad], although you must establish commercial relationships with graph partners directly, in order to leverage [!DNL Audience Manager]. All customers are expected to update any co-op Profile Merge Rules to utilize any options other than [!DNL Device Co-op.]

### [!DNL Real-time Customer Data Platform]

There are no plans to modify the current [!DNL Audience Manager Data Management Platform] (DMP). However, the deprecation of third-party cookies will likely create scale challenges for most DMP users. To help customers evolve their data management practices, Adobe is encouraging the reduction of dependencies on identifiers that will face restrictions in the coming year. Marketing teams must build first-party data strategies focused on durable identifiers that include personally identifiable information (PII), which can be solved for with [!DNL Real-time Customer Data Platform] (Real-time CDP).

[!DNL Real-time CDP] reduces dependencies on third-party cookies and device IDs by expanding the set of identifiers available for audience creation to include PII. Foundational to [!DNL Real-time CDP] is Real-time Customer Profile, which brings together person attribute data with behavioral data in real-time and allows marketers to create rich audience segments with patented data governance controls. Like [!DNL Audience Manager], [!DNL Real-time CDP] powers insights and personalization use cases, but also generates more granular person-level insights and can activate audiences to a broader range of destinations spanning advertising technologies and marketing technologies, including paid media, social media, email, and customer systems.

[!DNL Real-time CDP] will also include access to [Adobe Experience Platform Segment Match (Beta)](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-match/overview.html?lang=en), which allows brands to expand their own first-party data sets through partnerships and achieve improved insights and personalization.

### [!DNL Target]

There are currently no alternatives available for [!DNL Target] because [!DNL Target] provides a deterministic cross-device identity stitching capability known as `mbox3rdPartyId`, which functions similarly to Adobe's Customer ID. This capability allows [!DNL Target] customers to merge profiles and activity participation across [!DNL Target] tests and personalization being done in inbound channels.

### Adobe Advertising Cloud

[!DNL Advertising Cloud] customers will no longer be able to use [!DNL Device Co-op] for cross-device audience targeting and measurement. With [!DNL Advertising Cloud], you will still be able to leverage Adobe's [!DNL Device Graph] partnership with [!DNL LiveRamp] to continue to perform these functions to the extent of [!DNL LiveRamp's] ability and scale. You must allow your campaigns that are using [!DNL Device Co-op] to end, and then either switch to the [!DNL LiveRamp] device graph provider, or no longer leverage people-based targeting.

## What existing capabilities and implementations can help my preparation for a cookie-less future?

Your existing Visitor ID Service implementation powers Analytics [CDA](https://experienceleague.adobe.com/docs/analytics/components/cda/overview.html). If your existing declared ID is a hashed email, this can be used to power the following capabilities:

- [!DNL Audience Manager] [People-Based Destinations](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/destinations/people-based/people-based-destinations-overview.html).
- [Experience Platform Segment Match (Beta)](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-match/overview.html?lang=en).

## Will I get to keep my data from [!DNL Device Co-op]?

For [!DNL Audience Manager] and [!DNL Advertising Cloud] users, the data from [!DNL Device Co-op] will not be available to be transferred to third-party graphs. [!DNL Device Co-op] data will only be migrated for [!DNL Analytics Ultimate] users using CDA with [!DNL Device Co-op] switching to Field-Based Stitching. All other solutions will not have their data migrated.

## Is it mandatory to adopt other features?

While adoption of other Adobe features is not mandatory, you should start the implementation of other features as soon as possible to allow time and appropriate coordination in advance of [!DNL Device Co-op] deprecation.

## By when do I have to adopt alternative solutions if I choose to?

Adoption of other features is not mandatory. It is only recommended should you wish to continue addressing use-cases that were addressed by [!DNL Device Co-op]. If you choose to adopt other features, you must do so by 2022 (exact timing to be announced) before the [!DNL Device Co-op] program ends.

## How long will the adoption take?

This will depend on the feature. For example, if an Analytics Ultimate customer using Cross-Device Analytics with [!DNL Device Co-op] needs to migrate to Real-time Private Device Graph or Field-Based Stitching, adoption will take some time.

## What about the [!UICONTROL People] metric?

With the deprecation of the [!DNL Device Co-op], the [!UICONTROL People] metric is no longer relevant. On May 8, 2023, we will remove the [!UICONTROL People] metric. At that point, we will redirect its data to the [!UICONTROL Unique Visitor] metric in Analytics to prevent projects, segments and calculated metrics from breaking.

