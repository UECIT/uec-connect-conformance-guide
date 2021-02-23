---
title: Registering with the MAIT portal and EMS UI
keywords: development, versioning
tags: [development]
sidebar: overview_sidebar
permalink: register-with-mait-portal-and-ems-ui.html
summary: A guide on how to register with the MAIT Portal and EMS UI.
toc: true
---

## Introduction to the MAIT portal

The MAIT Portal is hosted within the NHS Digital OpenTest environment and for the purposes of UEC Connect testing has the following features:

*   Establishes a supplier account and provides details to enable registration of an EMS User Interface (UI) account
*   Enables registration of a supplier account with the EMS UI, and returns the login details, JSON Web Token, and endpoints to the user
*   Validation reports are viewable of submitted testing data 
*   Automated emailing of validation reports can be enabled for suppliers

_Note: NHS Digital staff have access to all supplier validation logs generated while communicating with the service to maintain and administer the service. Validation logs are isolated and private between supplier user accounts.  Under no circumstances should any Personally identifiable Data (PID) or other such 'live' data be submitted to the testing service. If you have any queries about this please contact us through the appropriate [Communication Channels](/support-communications.html)._

## Registering with the MAIT portal

1.  To access the MAIT portal you must first be connected to the NHS Digital OpenTest VPN. Complete this step (including registering if needed) before proceeding.
2.  Navigate to [http://192.168.128.17/Account/Register.aspx](http://192.168.128.17/Account/Register.aspx) to access the user registration form.
3.  Log in to the registration form using the details:
    1.  Username - admin
    2.  Password - ems
![MAIT admin login](/images/mait-admin-login.png)
4.  Complete the registration form taking care to enter a valid email address.
    1.  The first portion of your email address and the Supplier Name will be used as a unique identifier for your Mait login, EMS UI login and be tied to your validation reports
    2.  On successful form submission, your MAIT Portal account will be created and you can proceed to login
![MAIT registration form](/images/mait-registration-form.png)
5.  Access the user login page at [http://192.168.128.17/Account/Login.aspx](http://192.168.128.17/Account/Login.aspx) and use the credentials you set up in step 4 to log in.
6.  You have now successfully registered your account with the MAIT Portal



## Registering with the UEC Connect Test Harness

1.  After successfully logging into the MAIT Portal you will see an expanded menu on the left-hand side.
2.  Click the 'My EMS Token' option to view the EMS Registration Details screen.
3.  On initial visit, the page will be blank with two buttons: 'Register EMS Token' and 'Reset EMS Token'
4.  Click Register EMS Token to register new supplier details with the EMS UI.
5.  After a moment you will see the EMS Registration Details populated:
![MAIT EMS Registration](/images/mait-ems-registration.png)
6.  You have now successfully registered with the UEC Connect Test Harness.

## Reset your EMS Token

If for any reason you wish to reset your EMS Token, please follow these steps:

1.  Log in to the MAIT Portal with the user account details you registered.
2.  Navigate to the My EMS Token page
3.  Click the 'Reset EMS Token' button
    1.  The EMS UI and elastic search password will be reset and a new one generated on screen
    2.  The JWT token will be reset and a new one generated on screen
    3.  No other details will be changed

If you wish to change your Supplier account details or change any other settings you can return to the User Registration process to create a new MAIT Portal account.

## UEC Connect Test Harness endpoints

A set of details will be returned from the EMS UI when successfully registering.

<table>
<thead>
  <tr>
    <th style="width: 15%;">Name</th>
    <th style="width: 40%;">Detail</th>
    <th>Purpose</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>User Name</td>
    <td>&lt;system generated username&gt;</td>
    <td>User name to use when logging in to the EMS UI and the Elastic Search console.</td>
  </tr>
  <tr>
    <td>Password</td>
    <td>&lt;system generated password&gt;</td>
    <td>The password to use when logging in to the EMS UI and the Elastic Search console.</td>
  </tr>
  <tr>
    <td>JWT</td>
    <td>&lt;system generated JWT token&gt;</td>
    <td>Security token to use when communicating with the EMS and CDSS test instances. This must be included in the Authorization header for any messages sent by the supplier system to avoid the message being rejected.<br><a href="https://developer.nhs.uk/apis/cds-api-2-0-0/api_security.html">Security implementation guidance for developers</a></td>
  </tr>
  <tr>
    <td>Email</td>
    <td>&lt;Email you registered with&gt;</td>
    <td>Supplier email used when registering with the MAIT Portal. Used in part to generate the username and JWT token.<br>Also used if you have requested email validation reports.</td>
  </tr>
  <tr>
    <td>Logs</td>
    <td><a href="https://search-cactus-prod-audits-jspamsafneil44eui4rn5vabsa.eu-west-2.es.amazonaws.com/_plugin/kibana/">https://search-cactus-prod-audits-jspamsafneil44eui4rn5vabsa.eu-west-2.es.amazonaws.com/_plugin/kibana/</a></td>
    <td>URL to access the Elastic Search console for viewing interaction logs. Use the supplied Username and Password to log in.</td>
  </tr>
  <tr>
    <td>CDSS</td>
    <td><a href="https://cdss-1-1.uec-connect.nhs.uk/fhir">https://cdss-1-1.uec-connect.nhs.uk/fhir</a></td>
    <td>UEC Connect v1.1 CDSS test instance endpoint</td>
  </tr>
  <tr>
    <td>EMS</td>
    <td><a href="https://ems.uec-connect.nhs.uk/fhir">https://ems.uec-connect.nhs.uk/fhir</a></td>
    <td>UEC Connect EMS test instance endpoint</td>
  </tr>
  <tr>
    <td>EMSUI</td>
    <td><a href="https://ems-ui.uec-connect.nhs.uk/">https://ems-ui.uec-connect.nhs.uk</a></td>
    <td>URL to access the EMS User Interface.<br>Log in with the user name and password generated above.</td>
  </tr>
  <tr>
    <td>CDSS2</td>
    <td><a href="https://cdss-2-0.uec-connect.nhs.uk/fhir">https://cdss-2-0.uec-connect.nhs.uk/fhir</a></td>
    <td>UEC Connect v2.0 CDSS test instance endpoint</td>
  </tr>
  <tr>
    <td>DOS</td>
    <td><a href="https://dos.uec-connect.nhs.uk/fhir">https://dos.uec-connect.nhs.uk/fhir</a></td>
    <td>UEC Connect Directory of Services test instance endpoint</td>
  </tr>
</tbody>
</table>

You can access your registration details at any time by logging in to the MAIT portal and accessing the My EMS Token page.

## Next steps

After successfully registering with the EMS UI you can proceed to set up the relevant endpoints within your system.

You may now proceed to the [EMS UI](https://ems-ui.uec-connect.nhs.uk) to continue your setup.

Learn more about the [EMS test harness and how to log in](ems-cdss-overview.html) on the overview page.