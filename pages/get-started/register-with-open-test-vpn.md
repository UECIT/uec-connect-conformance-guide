---
title: Register with the OpenTest VPN
keywords: development, versioning
tags: [development]
sidebar: overview_sidebar
permalink: register-with-open-test-vpn.html
summary: A quick start reference guide for new users of the UEC Connect test tooling, from the perspective of an EMS or CDSS supplier.
toc: false
---


You must first request a VPN login and obtain a certificate in order to connect to the OpenTest environment - NHS Digital’s open-access network for developing healthcare applications.

You can find out more information on the [OpenTest environment on the NHS Digital website](https://digital.nhs.uk/services/spine/open-access-test-environment-for-spine-opentest).

_Note: While OpenTest can be used in the development of [Spine-related services](https://digital.nhs.uk/services/spine), UEC Connect testing does not require Spine connectivity and therefore OpenTest access may not automatically provide Spine access._

Connecting to OpenTest allows you to access the MAIT portal, where you can [register with the EMS UI](/register-with-mait-portal-and-ems-ui.html) and [view validation reports](/register-with-mait-portal-and-ems-ui.html).


## How to connect to the OpenTest environment

Before you start you will need to request an Opentest connection pack from [platforms.supportdesk@nhs.net](mailto:platforms.supportdesk@nhs.net). This pack will contain:
* A VPN token and credentials
* Predefined messaging endpoint
* Necessary certificates
* 2 MESH mailboxes

Opentest is a closed environment accessible only via the VPN token supplied, with predefined endpoints and products.

_For the purposes of UEC Connect testing, only the VPN token is needed to gain access to the environment. The Spine endpoint and MESH mailboxes are not required._

Within the connection pack you will need the included VPN client configuration file to connect, and OpenVPN client software. This can be downloaded from [http://openvpn.net](http://openvpn.net) and both graphical and command-line versions are available for a variety of operating systems including Linux, OSX and Windows. VPN login authentication is via a certificate in the included OVPN file.

OpenTest allows connections between endpoints. That means that you are responsible for protecting your own system, and for behaving in a responsible manner.

Full instructions for connecting are within the OpenTest connection pack.

## Maintenance slots and scheduled changes

The OpenTest environment is updated to the latest live baseline on a monthly basis. Find out [details of planned changes](https://digital.nhs.uk/services/path-to-live-environments/forward-change-schedule) and how these will impact on environment availability. 

After connecting to OpenTest you can proceed to [register with the MAIT portal and EMS UI](/register-with-mait-portal-and-ems-ui.html).