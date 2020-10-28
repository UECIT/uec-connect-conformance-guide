---
title: Quick start guide
keywords: development, versioning
tags: [development]
sidebar: overview_sidebar
permalink: quick-start-guide-ems-and-cdss.html
summary: A quick start reference guide for new users of the UEC Connect test tooling, from the perspective of an EMS or CDSS supplier.
toc: false
---

## Overview

The following list itemises the steps you must take to register with and then connect to the test tooling. Once connected, message interactions will be captured and you will be able to view message logs, call audits and validation reports. 

<table class="relative-table wrapped confluenceTable" style="" resolved="">
    <colgroup>
        <col style="width: 2.61324%;">
            <col style="width: 33.1978%;">
                <col style="width: 63.976%;">
                </colgroup>
                <tbody>
                    <tr>
                        <td class="numberingColumn confluenceTd"><p>1</p></td>
                        <td class="confluenceTd">
                            <p><a href="/register-with-open-test-vpn.html">Request a VPN login and connect to the OpenTest VPN</a></p>
                        </td>
                        <td class="confluenceTd">
                            <p>You must first request a VPN login and obtain a certificate in order to connect to the OpenTest environment.
                            </p>
                            <p>Connecting to OpenTest allows you to access the MAIT portal.</p>
                            <p><em>Note: You may already have an OpenTest account if you have previously performed testing with Spine.</em></p>
                        </td>
                    </tr>
                    <tr>
                        <td class="numberingColumn confluenceTd"><p>2</p></td>
                        <td class="confluenceTd">
                            <p><a href="/register-with-mait-portal-and-ems-ui.html">
                                                            Register an account with the MAIT portal and EMS User Interface
                                                        </a></p>
                        </td>
                        <td class="confluenceTd">
                            <p>Successfully connecting to OpenTest will allow you to access the MAIT portal. The portal allows you to register with the EMS UI and provides you with account and connection details.</p>
                            <p>Validation reports are also viewed within the MAIT portal.</p>
                        </td>
                    </tr>
                    <tr>
                        <td class="numberingColumn confluenceTd"><p>3</p></td>
                        <td class="confluenceTd">
                            <p>
                                <a href="/ems-overview.html">Connect to the test harness and use the EMS UI</a>
                            </p>
                        </td>
                        <td class="confluenceTd">
                            <p>Registering with the EMS UI (via the MAIT portal) will provide you with login details and system endpoints.</p>
                            <p>EMS Supplier</p>
                            <ul>
                                <li>Registering your system endpoint with the EMS is primarily to capture message interactions for the purposes of logging and validation. Registration of the CDSS test instance would be within your own system.</li>
                            </ul>
                            <p>CDSS Supplier</p>
                            <ul>
                                <li>Registering your system endpoint with the EMS allows discovery of your ServiceDefinitions and to perform a triage. Message interactions will be captured for logging and validation.</li>
                            </ul>
                        </td>
                    </tr>
                    <tr>
                        <td class="numberingColumn confluenceTd"><p>4</p></td>
                        <td class="confluenceTd">
                            <p>
                                <a href="/view-logs.html">Access and view message logs</a>
                            </p>
                        </td>
                        <td class="confluenceTd">Registering with the EMS UI (via the MAIT portal) provides you with an account on the ElasticSearch instance. Message interactions, once logged will be available to explore here.</td>
                    </tr>
                    <tr>
                        <td class="numberingColumn confluenceTd"><p>5</p></td>
                        <td class="confluenceTd">
                            <p>
                                <a href="/requesting-a-validation-report.html">Generate test evidence</a>
                            </p>
                        </td>
                        <td class="confluenceTd">The validation tab within the EMS UI allows you to select individual message interactions for validation.&nbsp;</td>
                    </tr>
                    <tr>
                        <td class="numberingColumn confluenceTd"><p>6</p></td>
                        <td class="confluenceTd">
                            <p>
                                <a href="/register-with-mait-portal-and-ems-ui.html">View validation reports</a>
                            </p>
                        </td>
                        <td class="confluenceTd">Message interactions sent for validation are available to view within the MAIT portal.</td>
                    </tr>
                </tbody>
            </table>