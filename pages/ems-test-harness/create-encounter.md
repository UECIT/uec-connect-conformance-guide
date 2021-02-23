---
title: Create an Encounter with the EMS UI
keywords: development, versioning
tags: [development]
sidebar: overview_sidebar
permalink: create-encounter.html
summary: A guide on how to create an Encounter with the EMS UI.
toc: true
---

## Encounter creation

After [logging in to the EMS UI](ems-cdss-overview.html) you will be presented with the initial triage screen. This allows you to create a new encounter for a patient with various scenario options configurable.

![ems test harness user interface](/images/ems-test-harness-user-interface.png)

## Patient selection

![ems patient selection](/images/ems-patient-selection.png)

Existing patients registered with the EMS can be selected from the grid. Additionally, it is possible to search for encounters with patients in an external EMS. The list of external EMS instances is configurable in the [EMS admin settings](ems-manage-settings.html).

Selecting an existing encounter through this dialogue will start the [encounter handover](handover.html) procedure.

![ems encounter report search](/images/ems-encounter-report-search.png)

## Encounter Context

### Setting

![ems select setting context](/images/ems-select-setting-context.png)

'Setting' is where the encounter takes place. Currently, there are three options:

*   Online implies that a patient or related person is interacting with the system directly
*   Phone call implies that a practitioner will be acting as an intermediary between the patient or related person and the EMS
*   Face to Face represents an in-person interaction between a patient or related person and a clinician

### User Type

![ems select receiving user type](/images/ems-select-receiving-user-type.png)

The encounter indicates an initiating and receiving person to indicate the type of user operating the system, and who will be receiving care advice respectively:

*   Patient is the individual who is being triaged during the encounter
*   Related person is an individual separate to the patient who is interacting with the encounter on their behalf
*   A practitioner is a professional working for the service provider who is managing the encounter

If 'online' is selected for the setting, the initiating person will match the receiving person, otherwise, it will always be a practitioner.

The receiving user is always a patient or a related person.

### Practitioner

![ems select practitioner](/images/ems-select-practitioner.png)

If a practitioner should be part of the encounter (non-online settings, as above) then a choice of practitioner is available in the encounter configuration. Otherwise, this section will be automatically hidden.

### Jurisdiction

![ems select jurisdiction](/images/ems-select-jurisdiction.png)

CDSS ServiceDefinitions may be restricted to particular jurisdictions. The encounter configuration allows this to be tested by selecting the jurisdiction in which the encounter is taking place.

## ServiceDefinition Selection

### Mode

![ems service definition selection mode](/images/ems-service-definition-selection-mode.png)

The EMS is able to select a ServiceDefinition in one of two modes:

*   Automated - the EMS will attempt to select a ServiceDefinition based on the information it already knows about a patient. This will query all [registered CDSS instances](https://kepler.bjss.com/pages/viewpage.action?spaceKey=NCTH&title=EMS+User+Guide#EMSUserGuide-cdss-suppliers).  
    In practice, this is most likely to give specialised results when an encounter handover is performed, but it can also allow different initial triage questions based on known patient information such as age, gender or the current useContext.
*   Manual - the EMS will allow selection of a specific CDSS instance and ServiceDefinition, regardless of any context requirements which may be specified by that ServiceDefinition.

### Automated Selection

![ems automated select service definition](/images/ems-automated-select-service-definition.png)

In Automated mode, a column will be shown for each registered CDSS, with available ServiceDefinitions shown. A single ServiceDefinition may be selected.

### Manual Selection

![ems manual select service definition](/images/ems-manual-select-service-definition.png)

In Manual mode, a toggle button will be shown for each registered CDSS instance. Selecting one will query that CDSS for available ServiceDefinitions, and display the list as a dropdown.

## Start Triage

Once a valid ServiceDefinition has been selected, its details will be displayed in a structured document view at the bottom of the page. If you are happy with the currently selected options, clicking on 'Start Triage' will create the new encounter and initiate the triage process, communicating with the selected CDSS and presenting triage questionnaires.

![ems start triage](/images/ems-start-triage.png)

Next: [Triage](triage.html)
