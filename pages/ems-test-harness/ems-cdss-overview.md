---
title: EMS and CDSS Test Harness Overview
keywords: development, versioning
tags: [development]
sidebar: overview_sidebar
permalink: ems-cdss-overview.html
summary: A guide on how to register with the MAIT Portal and EMS UI.
toc: true
---

## Overview

The UEC Connect [EMS](https://developer.nhs.uk/apis/cds-api-2-0-0/overview_concepts.html#encounter-management-system-ems) and [CDSS](https://developer.nhs.uk/apis/cds-api-2-0-0/overview_concepts.html#clinical-decision-support-system-cdss) Test Harness have been developed by NHS Digital primarily to inform the development of the UEC Connect Implementation Guide by acting as functional test instances utilising the UEC Connect standard.  Additionally, the test harness provides:

*   An open-sourced code base for the EMS and CDSS test implementations for interested suppliers
*   A platform for Suppliers to connect their systems to EMS and CDSS test implementation endpoints
*   A way to generate and collect technical evidence for the UEC Connect conformance process

## Open Source implementations

*   The code base for the test harness is [available on GitHub](https://github.com/UECIT).
*   Read more about the NHS England policy on open-source first - [https://www.england.nhs.uk/digitaltechnology/open-source/](https://www.england.nhs.uk/digitaltechnology/open-source/).

## Key features of the EMS Test harness

*   Support v1.1 interactions
    *   Select ServiceDefinition
    *   Evaluate
*   Support v2.0 interactions
    *   IsValid
    *   Check-Services
    *   Encounter Report
*   Message logging
*   Triage Audit reports
*   FHIR Message validation via the TKW Service

### Key absent features:

*   Backward navigation within the triage process
*   Registering of custom Directories
*   Any other simulation of national services (e.g. RCS, PDS) as this is out of scope of UEC Connect conformance

_Note: The EMS Test Harness is for demonstration purposes only and is not representative of any EMS final product._

## Key features of the CDSS Test harness

*   Two instances of CDSS covering both version 1.1 and version 2.0 of the implementation guide
*   Multiple sample ServiceDefinitions covering 
    *   A 'null' ServiceDefinition
    *   18 other ServiceDefinitions 
*   4 differing clinical scenarios
*   A range of question types and triage outcomes to exercise the EMS
*   Published endpoints for the CDSS to be consumed by an EMS supplier

_Note: The CDSS Test Harness is for demonstration purposes only and is not representative of any CDSS final product._

## Essential concepts for understanding the EMS UI

Before interacting with the EMS UI it is recommended to review the below topics within the UEC Connect 2.0 Implementation Guide. This will familiarise yourself with the core concepts of the API and the functionality of the UEC Connect 2.0 compliant version of the EMS UI.  

*   [Overview of concepts](https://developer.nhs.uk/apis/cds-api-2-0-0/overview_concepts.html)
*   [Overview of interactions](https://developer.nhs.uk/apis/cds-api-2-0-0/solution_interactions.html)
*   [Service Validity interaction](https://developer.nhs.uk/apis/cds-api-2-0-0/api_post_isvalid.html)
*   [Select ServiceDefinition interaction](https://developer.nhs.uk/apis/cds-api-2-0-0/api_get_service_definition.html) 
*   [Evaluate ServiceDefinition interaction](https://developer.nhs.uk/apis/cds-api-2-0-0/api_post_evaluate.html)
*   [Evaluate Response interaction](https://developer.nhs.uk/apis/cds-api-2-0-0/api_return_guidance_response.html)
*   [Check Services interaction](https://developer.nhs.uk/apis/cds-api-2-0-0/api_check_services.html)
*   [Encounter Report interaction](https://developer.nhs.uk/apis/cds-api-2-0-0/api_encounter_report.html)

## Login to the EMS UI

The EMS UI is hosted at [ems-ui.uec-connect.nhs.uk](https://ems-ui.uec-connect.nhs.uk/)

* Log in to the EMS using the username and password obtained from the registration process. See the [Quick start guide](/quick-start-guide-ems-and-cdss.html) for more details.

![EMS Login](/images/ems-login.png)

After logging in you will be presented with the initial triage screen. This allows you to create a new encounter for a patient with various scenario options configurable.

![EMS User Interface](/images/ems-test-harness-user-interface.png)

Next: [Create an Encounter](/create-encounter.html)