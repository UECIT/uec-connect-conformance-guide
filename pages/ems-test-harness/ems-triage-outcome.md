---
title: EMS triage outcome
keywords: development, versioning
tags: [development]
sidebar: overview_sidebar
permalink: ems-triage-outcome.html
summary: Achieving a triage outcome using the EMS UI.
toc: true
---

## Triage result

Results are shown when the CDSS returns Referral Requests or Care Plans. If the result is interim then the details will be displayed alongside the next questionnaire as per the normal triage.

For the final result, like the triage flow, the user can opt to end the test or switch suppliers. However, the user can no longer continue the triage as the encounter has been completed.

The user can switch between the 'Result Details' and 'Care Advice' tabs to view the Referral Request and Care Plan details respectively.

For the referral request, the user can select primary concern to view more details about it.

At the bottom of this page, the user can perform a search for services using the referral request that was issued by the CDSS.

![ems result details](/images/ems-result-details.png)

## Referrals
On the results page, the user can opt to search for services with the issued results. The user then has the option to view details about each of the services returned or invoke the service.

If the service selected is configured to handover to itself (i.e. the same instance of the EMS), then a handover is performed.

Note: The results returned are examples only and are not functional with the exception of the Handover service.

![ems service search](/images/ems-service-search.png)

Next: [Handover](handover.html)