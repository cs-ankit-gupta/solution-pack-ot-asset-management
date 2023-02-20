| [Home](../README.md) |
|--------------------------------------------|

# Contents

The **OT - Asset Management** solution pack contains the following resources.

## Dashboards

|Name|Description|
| :- | :- |
|  Asset Change Activity Tracking  |  Track the activity over asset change |
| Asset Overview | This dashboard displays Assets By Level, By Zone, By Vendor By Category, By Level By State, By Type, By Vendor, By MEF Tag  |
| Asset Risk Overview | Displays the alerts over assets By Zone, By Criticality, and Recent Alerts |

## Connectors

|Name| Version | Description|
| :- | :- | :- |
| CSV Data Management | 1.1.0 or later | CSV Data management can perform different operations on CSV files like reading files, performing deduplication, merging two CSV files, joining two CSV files, concatenation of two CSV files, and returning a well-formatted dataset |
| Fortinet FortiEDR | 1.3.0 or later | FortiEDR protects endpoints pre and post-infection, stopping data breaches in real-time and automatically orchestrating incident investigation and response. This connector facilitates automated operations related to events, forensics, and collectors. |
| Fortinet FortiGate | 5.2.1 or later | Fortinet FortiGate enterprise firewall provides high performance, consolidated advanced security, and granular visibility for broad protection across the entire digital attack surface. |
| ServiceNow | 3.2.0 or later | ServiceNow connector provides functionality to create, read, update, and delete records of Table and Catalog type |
| Qualys | 1.0.1 or later | Qualys provides cloud security, compliance, and protection of IT assets and web applications. This connector facilitates automated operations for vulnerability management, policy compliance, and asset management. |
| MITRE ATT&CK > Fetch Latest Data | Manually fetches the latest data from MITRE |
## Widgets

|Name|Description|
| :- | :- |
| Record Distribution | Ability to visualize items/records and their correlations in different levels based on a given grouping context. A very good example of the widget's utility is the OT view, where assets are visualized across different Purdue Levels and highlight any existing relations with other assets at different levels. | 
| MITRE ATT&CK Alert Incident Spread | Detailed table view of Alerts and Incidents linked to MITRE ATT&CK records. |
 
## Module Schema

|Name|Description|
| :- | :- |
| Asset | New Fields have been added. Such as Network, Subnet, Firmware, ESPZone, Facility, Zone, Level, Vendor, Asset Type, Protocol, Assets, Vulnerability Risk Status, Asset Change Activity, and Asset Icon. |
| Asset Resources | A Module that contains the icons of assets |
| Asset Change Activity | A module that monitors asset changes on various baselines. |


## Picklist

|Name|
| :- |
| ActivityStatus |
| AssetChangeType |
| AssetCategory |
| AssetLevel |
| AssetProtocol |
| AssetType |
| AssetZone |
| VulnerabilityRiskStatus |

## Report

|Name|Description|
| :- | :- |
| Asset Change Activity Summary Report | Provide the report over asset change activity |


## Roles

|Name|Description|
| :- | :- |
|  Full App Permissions  |  Full App Permissions for the Asset Change Activity Module  |

## Scenario Record Set

|Name|Description|
| :- | :- |
| OT - Add Sample Assets | This scenario adds 83 different samples of OT Assets (different Purdue Levels, Types, etc.) for testing dashboards, use case playbooks, reports, and other actions. |
| OT - Add Sample Alerts | This scenario adds 12 well-populated samples OT Alerts for testing dashboards, use case playbooks, reports, and other actions. |
| OT - Stuxnet Attack Scenario | This scenario recreates the Stuxnet attack in form of a series of point alerts received by FortiSOAR from FortISIEM. |
| OT - Add Sample Asset Change Activity Record | This scenario generates a sample Asset Change Activity record each, for type "Add New Asset" and "Medium Impact Baseline Change" type of activities. |

## Asset Resources Record Set

|Name|Description|
| :- | :- |
| PLC | This contains the image file for the PLC icon. |
| WorkStation | This contains the image file for the WorkStation icon. |
| Laptop, Desktop, Endpoint | This contains the image file for Laptop, Desktop, and Endpoint icon. |
| Switch | This contains the image file for the Switch icon. |
| Server | This contains the image file for the Server icon. |
| Network | This contains the image file for the Network icon. |
| Router | This contains the image file for the Router icon. |
| HMI | This contains the image file for the HMI icon. |
| Firewall | This contains the image file for the Firewall icon. |
| Storage | This contains the image file for the Storage icon. |

## Playbook Collection

### 00 - Use Case - Asset Change Activity

|Playbook Name|Description|
| :- | :- |
| Scenario - OT - Asset Change Activity | Generate an Asset Change Activity record for type Add New Asset and Medium Impact Baseline Change. |
| Medium Impact Baseline Change | Baseline Change Workflow for Medium Impact Cyber Assets |
| High Impact Baseline Change | Baseline Change Workflow for High Impact Cyber Assets |
| Add Cyber Asset | Baseline Change Workflow for Add Cyber Asset |
| Remove Cyber Asset | Baseline Change Workflow for Remove Cyber Asset |
| Replace Cyber Asset | Baseline Change Workflow for Replace Cyber Assets |
| Modify Cyber Asset | Baseline Change Workflow for Modify Cyber Asset |
| Add New Task | New task for Asset Change Activity |
| Manage Asset Change Activity Closure | Update the "Closed On" field with the current date and time if the status is Closed. |
| Generate Asset Change Summary Report | Generate report by manual trigger in FortiSOAR |
| Generate Report | Generates Report and Link to Incidents |

### 00 - Use Case - Asset Management

|Playbook Name|Description|
| :- | :- |
| Scenario - OT - Create Assets Record | Playbook will read a CSV file and create Assets records. |
| Create Assets Record | This will generate an Alert record. |
| Set Assets With MEF Tag | This PB will add MEF tag on Assets. | 
| Scenario - OT - Create Alerts Record | Playbook will read a CSV file and create Alerts records. |
| Create Alerts Record | This will generate an Asset record. |
| Scenario - OT - Stuxnet Attack Scenario | Generate Alert for Stuxnet worm that targets Siemens S7 PLCs connected to Engineering Stations. |
| On Alert Creation | Based on the MITRE Technique used for Alert, link the Sub Technique, Mitigation, Software, and Group. |
| Find Assets | Finds the asset based on the IP address provided. |
| Alert - Escalate To Incident | Creates a new incident with the given inputs and links the alert(s) to the newly created Incident. |
| Alert - Escalate To Incident (No Trigger) | Creates a new incident with the given inputs and links the alert(s) to the newly created Incident. |
| Alert - Escalate to Incident (Link Relations) | This playbook extracts related records and assigns them to the incident created |
| Quarantine Asset and Raise Ticket | This playbook quarantines assets and raises a ticket. |
| Isolate and Comment Assets | This PB will update the assets as isolated and add a comment. |
| Update Firewall Policy | Update Firewall Policies To Restrict Communications. | 
| Scan All Assets Involved | Initiate a quick scan on all assets related to the incident. |
| Isolate Devices From Network | Isolate Selected Devices From Network Based On Criticality and Risk. |

## System View
|Name|
| :- |
| Navigation Structure - Resources |


>**Warning:** We recommend that you clone these playbooks before customizing to avoid loss of information while upgrading the solution pack.
