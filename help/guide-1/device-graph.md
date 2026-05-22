---
keywords: Device-graph;end-of-life
title: Device graph
description: Learn about the end-of-life plans for the Device graph.
---
# End-of-life for device graph

>[!WARNING]
>
>Device Graph within Cross-Device Analytics is no longer available as of **December 31, 2025**. Please switch any current device graph enabled virtual report suite to the [field-based method](https://experienceleague.adobe.com/en/docs/analytics/components/cda/field-based-stitching).

Cross-Device Analytics did use the Private Graph to stitch data together. The Private Graph is a repository of hashed device ID's that is specific to your organization. CDA regularly communicates with the device graph to link devices together.

## Prerequisites specific to the device graph

If you intended to implement Cross-Device Analytics using the device graph method, the following were required.

>[!WARNING]
>
>Failure to meet all prerequisites could result in the inability to enable Cross-Device Analytics or poor results when stitching data.

* Your organization must use the [Adobe Experience Platform Identity Service Private Graph](https://business.adobe.com/products/experience-platform/identity-service.html). See also the [Home Page](https://experienceleague.adobe.com/docs/experience-platform/identity/home.html) in the Identity Service user guide.
* Your implementation must use the latest version of the ID Service (ECID). See the [Home Page](https://experienceleague.adobe.com/docs/id-service/using/home.html) in the ID Service user guide. Most implementations using [Tags](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html) in Adobe Experience Platform likely already have ID Service deployed.
* Your implementation must call the `setCustomerIDs` function (or SDK equivalent) whenever an individual can be identified, such as when a user logs in or opens an email. This requirement applies to all platforms, including mobile apps if used. See [`setCustomerIDs`](https://experienceleague.adobe.com/docs/id-service/using/id-service-api/methods/setcustomerids.html) in the ID Service user guide.

## Limitations specific to the device graph

* Legacy Analytics IDs are not supported. Only visitors with ECIDs are stitched.
* If your organization uses a Private Graph, new devices take up to 24 hours to be stitched. 
* 3rd-party device graphs are not supported.

