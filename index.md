---
title: Introduction to the UEC Connect Conformance Guide
keywords: homepage
tags: [overview]
sidebar: overview_sidebar
permalink: index.html
toc: false
summary: A brief introduction to the UEC Connect Conformance Guide
---

## Introduction

This site is a usage guide for the test tools that support NHS Digital's [UEC Connect API standard](https://developer.nhs.uk/apis/cds-api/) (formally known as the CDS API) and the related UEC Connect conformance approach.

The test tools underpin the process for getting products certified under the UEC Connect conformance approach, but they will also be of use during general development of relevant products not being formally assessed for conformance. As such this guide has been written with a particular focus on assisting suppliers with the formal conformance process, but aspects it contains, such as interacting with the testing tools, can be used during a general product development stage.

The suite of test tools:

*   provides UEC Connect API endpoints, which can be utilised by suppliers to test the functionality of their Encounter Management System (EMS) or Clinical Decision Support System (CDSS)
*   provides various use case scenarios to allow suppliers to exercise their product and highlight compliance or non-compliance to the standard
*   features both CDSS and EMS test instances that suppliers can connect their system to
*   operates within an NHS Digital test environment
*   supports the capturing of log outputs and validation reports

The end result of using the test tools will be outputs clearly indicating whether or not a system is compliant to the UEC Connect specification:

*   where a system has been tested and found to be compliant, the logs and validation will provide essential technical evidence needed to gain Conformance certification
*   where non-conformance is identified, validation reports will identify the required areas for development in the supplier’s product to become conformant

## Intended audience

The intended users of this guide are primarily developers who are building systems compliant to the UEC Connect implementation guide [v1.1](https://developer.nhs.uk/apis/cds-api-1-1-0/) or [v2.0](https://developer.nhs.uk/apis/cds-api-2-0-0/). Consideration has also been given to product specialists involved in the design and testing of systems implementing the UEC Connect standard. The scope of the guide is therefore assets and information intended for a technical audience.

## In scope

The information in this site covers two broad categories:

### Onboarding of software suppliers to the UEC Connect test tools which provide:

*   A closed test environment for suppliers to register system endpoints
*   Sample EMS test instance
*   Sample CDSS test instance
*   Automated capture of interaction logs
*   Automated generation of validation reports
*   Support for the collection of technical test evidence

### Onboarding of software suppliers to the UEC Connect conformance process

*   An overview of the NHS Digital approach for UEC Connect conformance
*   UEC Connect conformance risk log
*   Test cases for validating key API functionality
*   Clinical Scenarios built in to the sample CDSS instance
*   Applying for conformance certification

## Out of scope

### Implementation guidance

The primary source of UEC Connect implementation guidance is within the [Implementation Guide](https://developer.nhs.uk/apis/cds-api-2-0-0/). This guide is restricted to user guidance for the test tooling and to support system suppliers through the conformance process.

### Example messages

Normative example messages and resources are not included in this version of the usage guide but will be added when available.

## Useful Links 

*   UEC Connect test tools: Quick start guide for EMS and CDSS suppliers
*   [EMS Test Harness - User Interface](https://ems-ui.uec-connect.nhs.uk/)(account required)
*   [Open Test MAIT Portal](http://192.168.128.17/Account/Login.aspx) (VPN required)
*   [UEC Connect Implementation Guide v1.1]((https://developer.nhs.uk/apis/cds-api-1-1-0/))
*   [UEC Connect Implementation Guide v2.0]((https://developer.nhs.uk/apis/cds-api-2-0-0/))
*   [Solution Concepts](https://developer.nhs.uk/apis/cds-api-2-0-0/overview_concepts.html)
*   [Solution Interactions](https://developer.nhs.uk/apis/cds-api-2-0-0/solution_interactions.html)

## Note for Implementers

This guide is issued as an alpha, and we welcome feedback (see Communication Channels for ways to contact us) on the guide and suggestions for improvement.