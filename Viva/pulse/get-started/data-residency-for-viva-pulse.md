---
title: Data residency for Viva Pulse
description: "Data residency for Viva Pulse"
ms.reviewer: 
ms.author: michellehu
author: michellehu-msft
manager: alisaliddle
audience: Admin
f1.keywords: NOCSH
ms.date: 07/12/2023
ms.topic: article
ms.service: viva
ms.subservice: viva-pulse
ms.localizationpriority: medium
ms.collection: m365initiative-viva-pulse  
search.appverid: MET150
---

# Data residency for Viva Pulse

## Summary

Service documentation: [Microsoft Viva Pulse overview](../introduction-to-viva-pulse.md)

Viva Pulse empowers leaders and managers to seek and act on feedback when it matters. Using research-backed templates, teams can quickly share their experience and suggestions, and reporting helps managers pinpoint what is working well and which areas to focus on over time.  

## Multi-geo capabilities in Viva Pulse

Multi-geo capabilities for Viva Pulse are limited to two regions, West US and EU, for data stored at rest which constitutes metadata for the Pulses authored and responded to, as well as reports generated for those Pulses. The Pulse instances and the responses are stored in Microsoft Forms, where the data residency for Forms becomes applicable.

**West US data residency**

Required conditions:
1. _Tenant_ has a sign-up country that is non-EU.
2. _Tenant_ has a valid Viva Pulse license.  
3. _Tenant_ has a valid Microsoft Forms license.

**EU data residency**

Required conditions:
1. _Tenant_ has a sign-up country included in European Union Data Boundary (EUDB). 
2. _Tenant_ has a valid Viva Pulse license.
3. _Tenant_ has a valid Microsoft Forms license.

## User experience

Viva Pulse multi-geo is seamless to the end user. The application will appropriately redirect the user to the correct region.

## How can I determine customer data location?

Viva Pulse research-backed templates and customized templates are stored in Azure Cosmos DB in West US or EU depending on the tenant’s billing location. Pulse instances authored in Viva Pulse are stored in Microsoft Forms, along with all the responses to the Pulse. Data in Microsoft Forms is subject to [data residency capabilities offered by Microsoft Forms](https://support.microsoft.com/office/data-storage-for-microsoft-forms-97a34e2e-98e1-4dc2-b6b4-7a8444cb1dc3).