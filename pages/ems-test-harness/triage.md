---
title: Registering with the MAIT portal and EMS UI
keywords: development, versioning
tags: [development]
sidebar: overview_sidebar
permalink: triage.html
summary: A guide on how to register with the MAIT Portal and EMS UI.
toc: true
---

## Triage

After selecting 'Start Triage' in the [Create an Encounter view](https://nhsd-confluence.digital.nhs.uk/display/CACT/Create+an+Encounter), the EMS contacts the selected CDSS and initiates the triage session. The CDSS will respond with a Questionnaire which should be answered by the user of the EMS.

![ems triage ui](/images/ems-triage.png)

The Triage view shows the following features:

1.  Patient information
2.  List of questions previously answered during the encounter
3.  Current Questionnaire
4.  Current Service Definition
5.  Current CDSS instance
6.  Current user role
7.  Continue triage after answering the current questionnaire
8.  Switch Supplier allows a new CDSS and Service Definition to be selected
9.  End test returns to the home screen
10.  An audit log shows details of all interactions between the user and EMS during the encounter, and all further requests made by the EMS to other services.

## Answering Questions

Questions in several formats are supported by the UEC Connect standard. These include multiple-choice, text input, image map and file upload questions.

After selecting an answer (if required) you should click on the 'Continue' button (7) to submit the answer to the CDSS and proceed to the next step, which may be another Questionnaire, redirection to another ServiceDefinition, or a [triage result](results.html).

## Redirection and Switching Supplier

Occasionally the CDSS may indicate that the user should be redirected to another ServiceDefinition. This may be to allow a more specialised set of questions to be answered based on answers given to more general initial triage questions, or it may be that several presenting complaints lead to the same set of questions which are better captured in a single ServiceDefinition rather than repeated in several places.

When a redirection occurs, the user will be informed by the EMS using a pop-up confirmation dialog:

![ems switch service definition](/images/ems-switch-service-definition.png)

At any point during triage, the user can manually switch to a new ServiceDefinition by selecting 'Switch Supplier' (8). This will allow the user to select a new ServiceDefinition in the same way as the manual selection during encounter configuration.

![ems switch supplier](/images/ems-switch-supplier.png)

Next: Continuing the triage journey through a question set and any redirection to other ServiceDefinitions will result in an [outcome of triage](ems-triage-outcome.html).