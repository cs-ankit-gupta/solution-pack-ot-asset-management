| [Home](../README.md) |
|--------------------------------------------|

# Contents

The `OT - Asset Management` solution pack contains the following resources.

## Dashboards

|**Name**|**Description**|
| :- | :- |
|  Asset Change Activity Tracking  |  Track the activity over asset change activity |
| Asset Overview | This dashboard displays Assets By Level, By Zone, By Vendor By Category, By Level By State, By Type, By Vendor, By MEF Tag  |
| Asset Risk Overview | Display the alerts over assets By Zone, By Criticality, Recent Alert |

## Connectors

|**Name**| **Version** | **Description**|
| :- | :- | :- |
| CSV Data Management | 1.1.0 or later | CSV Data management can perform different operations on CSV files like read file, perform deduplication, merge two CSV files, join two CSV files, concat two CSV files and return well formatted dataset |
| Fortinet FortiEDR | 1.3.0 or later | FortiEDR protects endpoints pre and post infection, stopping data breaches in real-time and automatically orchestrating incident investigation and response. This connector facilitates the automated operations related to events, forensics and collectors. |
| Fortinet FortiGate | 5.2.1 or later | Fortinet FortiGate enterprise firewall provide high performance, consolidated advanced security and granular visibility for broad protection across the entire digital attack surface. |
| ServiceNow | 3.2.0 or later | ServiceNow connector provides functionality to create, read, update and delete records of Table and Catalog type |
| Qualys | 1.0.1 or later | Qualys provides cloud security, compliance and protection of IT assets and web applications. This connector facilitates the automated operations for vulnerability management, policy compliance, asset management. |
| MITRE ATT&CK > Fetch Latest Data | Manually fetches the latest data from MITRE |
## Widgets

|**Name**|**Description**|
| :- | :- |
| Record Distribution | Ability to visualise items/records and their correlations in different levels based on a given grouping context. A very good example of the widget's utility is the OT view, where assets are visualised across different Purdue Levels and highlight any existing relations with other assets at different levels. | 
| MITRE ATT&CK Alert Incident Spread | Detailed table view of Alerts and Incidents linked to MITRE ATT&CK records. |
 
## Module Schema

|**Name**|**Description**|
| :- | :- |
| Asset | New Fields has been added. Such as: Network, Subnet, Firmware, ESPZone, Facility, Zone, Level, Vendor, Asset Type, Protocol, Assets, Vulnerability Risk Status, Asset Change Activity, Asset Icon. |
| Asset Resources | A Module that contain the Icons of Assets |
| Asset Change Activity | A module that monitors asset changes on various baselines. |


## Picklist

|**Name**|
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

|**Name**|**Description**|
| :- | :- |
| Asset Change Activity Summary Report | Provide the report over asset change activity |


## Roles

|**Name**|**Description**|
| :- | :- |
|  Full App Permissions  |  Full App Permissions for the Asset Change Activity Module  |

## Scenario Record Set

|**Name**|**Description**|
| :- | :- |
| OT - Add Sample Assets | This scenario adds 83 different sample OT Assets (different Purdue Levels, Types etc.) for testing dashboards, use case playbooks, reports and other actions. |
| OT - Add Sample Alerts | This scenario adds 12 well populated sample OT Alerts for testing dashboards, use case playbooks, reports and other actions. |
| OT - Stuxnet Attack Scenario | This scenario recreates the Stuxnet attack in form of series of point alerts received by FortiSOAR from FortISIEM. |
| OT - Add Sample Asset Change Activity Record | This scenario generates sample Asset Change Activity record each, for type "Add New Asset" and "Medium Impact Baseline Change" type of activities. |

## Asset Resources Record Set

|**Name**|**Description**|
| :- | :- |
| PLC | This contain the image file for PLC icon. |
| WorkStation | This contain the image file for WorkStation icon. |
| Laptop, Desktop, Endpoint | This contain the image file for Laptop, Desktop, Endpoint icon. |
| Switch | This contain the image file for Switch icon. |
| Server | This contain the image file for Server icon. |
| Network | This contain the image file for Network icon. |
| Router | This contain the image file for Router icon. |
| HMI | This contain the image file for HMI icon. |
| Firewall | This contain the image file for Firewall icon. |
| Storage | This contain the image file for Storage icon. |

## Playbook Collection

### 00 - Use Case - Asset Change Activity

|**Playbook Name**|**Description**|
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

|**Playbook Name**|**Description**|
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
| Alert - Escalate to Incident (Link Relations) | This playbook will extract related records and assign to incident created |
| Quarantine Asset and Raise Ticket | This playbook quarantine assets and raise ticket. |
| Isolate and Comment Assets | This PB will update the assets as isolate and add a comment. |
| Update Firewall Policy | Update Firewall Policies To Restrict Communications. | 
| Scan All Assets Involved | Initiate a quick scan on all assets related to incident. |
| Isolate Devices From Network | Isolate Selected Devices From Network Based On Criticality and Risk. |

## System View
|**Name**|
| :- |
| Navigation Structure - Resources |


>**Warning:** We recommend that you clone these playbooks before customizing to avoid loss of information while upgrading the solution pack.
