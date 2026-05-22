---
title: Adobe Media SDK (versions 1.x and 2.x) end-of-life FAQ
description: Get answers to commonly asked questions about the end-of-life for Adobe Media SDK versions 1.x and 2.x (formerly Video Heartbeat Library).
---

# Adobe Media SDK (versions 1.x and 2.x) end-of-life FAQ

Adobe Media SDK **2.x reached end of support on August 31, 2021**. Video Heartbeat Library (VHL) **1.x is deprecated** and has not been supported for several years.

## What is happening?

The original Video Heartbeat Library (VHL), later renamed Media SDK, provided client-side tracking for audio and video analytics. Adobe has transitioned tracking capabilities to newer, more capable implementations:

* **Media SDK 3.x (Analytics-only):** Currently supported. Tracks media using the Media Collection API. Recommended for existing 2.x users who cannot yet move to the Edge Network.
* **Streaming Media for Edge Network (recommended):** The current recommended implementation. Uses the Adobe Experience Platform Web SDK, Mobile SDK, or Media Edge API to send media data through the Edge Network, enabling use across Adobe Analytics, Customer Journey Analytics, Real-Time CDP, and Adobe Journey Optimizer.

## What is included in end-of-life, and what is not?

**End-of-life (no longer supported):**

* Video Heartbeat Library (VHL) 1.x — all platforms (Android, iOS, JavaScript, Apple TV, Chromecast, Roku, TVML)
* Media SDK 2.x — Android, iOS, JavaScript

**Not end-of-life (still supported):**

* Media SDK 3.x — JavaScript, Chromecast, Roku (Analytics-only)
* Streaming Media for Edge Network — all supported platforms

## Why were versions 1.x and 2.x retired?

Starting with version 3.0, the Media SDK was redesigned to use the Media Collection API directly, eliminating the need for a delegate pattern and simplifying tracker creation. The older 1.x and 2.x SDKs relied on a heartbeat server architecture that has since been superseded.

Adobe also introduced the Edge Network implementation to provide a single data collection pipeline capable of feeding multiple downstream Adobe applications, which the legacy heartbeat SDKs could not support.

## Where can I find the archived documentation?

Legacy documentation has been archived on GitHub and is available for reference:

| Version | Status | Archived documentation |
|---|---|---|
| 1.x (Video Heartbeat Library) | Deprecated | [`video-heartbeat` GitHub repository](https://github.com/Adobe-Marketing-Cloud/video-heartbeat/tree/master/docs) |
| 2.x (Media SDK) | End of support Aug 31, 2021 | [`media-sdks` GitHub repository](https://github.com/Adobe-Marketing-Cloud/media-sdks/blob/master/docs/2.x/README.md) |

## What are my transition options?

**Option 1: Migrate to Media SDK 3.x (Analytics-only)**

If you are on 2.x and use Adobe Analytics exclusively, migrating to 3.x is the simplest path. See the [2.x to 3.x migration guide](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/media-sdk/setup/migrate-js-2x-to-3x.html) for a full API comparison and code examples.

**Option 2: Migrate to Streaming Media for Edge Network (recommended)**

For new implementations or when you want to use data across multiple Adobe applications, use the Adobe Experience Platform Edge Network:

* [Media Edge Web SDK](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/edge-web-sdk.html)
* [Media Edge Mobile SDK](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/edge-mobile-sdk.html)
* [Media Edge API](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/implementation-edge-api.html)

## FAQs

+++**Will support for Roku and Chromecast SDKs be impacted?**

No. The Roku and Chromecast SDKs remain available and supported as part of Media SDK 3.x (Analytics-only). This end-of-life covers only the 1.x and 2.x versions.

+++

+++**Will Media Analytics JavaScript SDK implementations be impacted?**

No. Customers who use the JavaScript SDK for Media Analytics can continue to use the standalone SDK or tag extension.

+++

+++**I am still on Media SDK 2.x. What should I do?**

Adobe recommends migrating to the Edge Network implementation for all new projects. If you need an intermediate step, [Migrate from JavaScript SDK 2.x to 3.x](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/media-sdk/setup/migrate-js-2x-to-3x.html), then plan your move to the Edge Network.

+++

+++**What is the level of effort to migrate to a supported implementation?**

Migration effort depends on each customer's implementation and will vary. After reviewing the migration documentation, engage consulting or customer care for additional support:

* [Implement Streaming Media using the Mobile Edge SDK — Android and iOS](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/edge-mobile-sdk.html)
* [Migrate from JavaScript SDK 2.x to 3.x](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/media-sdk/setup/migrate-js-2x-to-3x.html)

+++

+++**Do I need to use Adobe Experience Platform Tags as a tag management system?**

For mobile app implementations, Experience Platform Tags is not used as a tag management system the way it is for web. The Tags UI is required for configuring SDK extensions. This is similar to how the Adobe Mobile Services UI was used to configure the Mobile v4 SDK. Tags provides customized installation instructions based on the extension you choose.

+++

+++**Does this end of support impact the SDK for tvOS?**

Yes. For tvOS (version 10+) the recommended implementation is to migrate to Streaming Media for Edge Network using the Adobe Experience Platform Mobile SDK. See [Implement Streaming Media using the Mobile Edge SDK](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/edge-mobile-sdk.html) for details.

+++

+++**Does this end of support impact the SDK for Fire TV and Android TV?**

Yes. For Fire TV and Android TV, the recommended implementation is to migrate to Streaming Media for Edge Network using the Adobe Experience Platform Mobile SDK. See [Implement Streaming Media using the Mobile Edge SDK](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/edge-mobile-sdk.html) for details.

+++

+++**Where can I find the Mobile v4 SDK end-of-life information?**

See the [Mobile Services end-of-life FAQ](mobile-services.md). The Mobile Services platform and Mobile v4 SDKs reached end-of-life on December 31, 2022.

+++

+++**Where can I go if I have questions?**

Contact your Adobe account team or Adobe Customer Care for migration assistance.

+++

>[!MORELIKETHIS]
>
>* [Streaming Media implementation overview](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/overview.html)
>* [Streaming Media for Edge Network](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/implementation-edge.html)
>* [Media SDK 3.x — JavaScript setup](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/media-sdk/setup/web-implementation.html)
