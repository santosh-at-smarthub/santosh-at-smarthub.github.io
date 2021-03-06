---
title: "Release Notes - 2020.09"
permalink: /docs/en/INFER-IoT-Center/2020.09/INFER-IoT-Center-202009-Release-Notes.html
excerpt: "SmartHub INFER IoT Center Release Notes"
last_modified_at: September 21, 2020
toc: true
---

|Release Name  | Version |
|--|--|
| SaaS |  2020.09-100003|
|On-premise|3.0.0-100003|
|Agent|3.0.0-100003|

### About SmartHub INFER IoT Center

> SmartHub INFER IoT Center is a secure, enterprise-grade, edge and IoT solution that provides visibility and control over all IoT use cases. It helps companies to onboard, configure, monitor, manage and secure IoT devices and infrastructure. The solution enables IT and Operational Technology (OT) to simplify device management and operationalize IoT use cases quickly by reducing the complexity of managing all the heterogeneous edge and IoT systems in one place.

SmartHub INFER IoT Center includes the following features and capabilities:

#### Onboard

- Onboard certified gateways and connected devices securely to the Service Offering through a low-touch enrollment process 
- Configure gateways, connectivity to gateways, and application/containers on gateways 
- Setup of device properties and metrics through device template 
- Define metrics collection frequency and batch size

#### Monitor and Troubleshoot IoT Infrastructure

- Set up alert definition and notification through email or REST API
- Monitor device health and detect abnormalities
- Troubleshoot through system log and audit log
- Act by sending supported commands to devices

#### Manage IoT Infrastructure

- Enable policy-driven over-the-air software lifecycle management
- Manage the software and security patch update approval process
- View alerts, metrics trends, and granular status of software update execution on the dashboard
- Visualize the representation of the parent-child topology
- Manage certified heterogeneous devices and gateways with different hardware, operating systems, and communication protocols

#### Interface

- Role-based user access according to organizations and use cases.


### New in this Release

- Re-branded with a fresh look
- Powerful insights and visualization of metrics and properties
- Newly introduced data lake where you can bring in external data to combine with device data for rich dashboards
- Easily integrate your Single Sign On (SSO)
- You can now use the SAML SSO to authenticate user access
- Simply provide OTA updates to new things and sub-organizations
- Perform OTA updates on ‘Thing devices’ that are enrolled after the campaign starts.
- OTA Campaigns now support Organization hierarchy.
- Richer and more convenient Advanced Search
- You can now search across multiple templates in Advanced Search.
- Organization is now visible in Advanced Search results.
- Automatic update of device lists for Alert Definitions
- Periodic background evaluation of search filter criteria to automatically add or remove devices in device list based Alert Definitions.
- Robust Load Balancing with High Availability (HA)
- You can now deploy Load Balancer in Active-Passive Mode to enable HA.


### Devices Certified for Use  

SmartHub’s Compatibility Guide lists the Gateways and Edge Systems that are certified for use with SmartHub INFER IoT Center:

-  [IoT & Edge Gateways](/docs/en/INFER-IoT-Center/compatibility/certified-edge-gateways)
-  [Embedded Systems](/docs/en/INFER-IoT-Center/compatibility/certified-embedded-systems)


### Before You Begin

Before you begin using SmartHub INFER IoT Center, ensure the following:

- Setup the following under **Identity & Access**
- Add the appropriate **Organization**. If you have more than one Organization, use the *Org Switcher* drop-down at the top-left of the page to change your current context.
- Review the pre-defined **Roles** and make any changes as needed
- Review/Edit/Create **Groups** with appropriate Roles to suit your needs
- Add **Users** to the system
- Ensure that your devices are certified for use with SmartHub INFER IoT Center

  
Please refer to detailed steps provided in the **User Guide** available under the *Help* menu on the top right corner of the SmartHub INFER IoT Center Console.


### Known Issues

The following known issues will be fixed in the upcoming releases:

- The agent config file does not get updated when you delete all the proxy configurations in the template.
- After enrolling a gateway, edit the device template with proxy settings and check the agent config file. The proxy settings are updated. When you delete all the proxy settings in the template, the agent config file does not update the changes.
- Add a proxy setting with an invalid proxy IP address. This will update the proxy type in the agent config file to NO\_PROXY.