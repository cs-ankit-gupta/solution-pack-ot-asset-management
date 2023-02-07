| [Home](../README.md) |
|--------------------------------------------|

# Contents

The `OT - Asset Management` solution pack contains the following resources.

## Dashboards

|**Name**|**Description**|
| :- | :- |
|  Asset Change Activity Tracking  |  Track the activity over asset change activity |
| Asset Overview | This dashboard displays Assets By Purdue Level, By Purdue Zone, By Vendor By Category, By Level By State, By Type, By Vendor  |
| Asset Risk Overview | Display the alerts over assets By Zone, By Criticality, Recent Alert |

## Connectors

|**Name**| **Version** | **Description**|
| :- | :- | :- |
| CSV Data Management | 1.1.0 or later | CSV Data management can perform different operations on CSV files like read file, perform deduplication, merge two CSV files, join two CSV files, concat two CSV files and return well formatted dataset |
| Fortinet FortiEDR | 1.3.0 or later | FortiEDR protects endpoints pre and post infection, stopping data breaches in real-time and automatically orchestrating incident investigation and response. This connector facilitates the automated operations related to events, forensics and collectors. |
| ServiceNow | 3.2.0 or later | ServiceNow connector provides functionality to create, read, update and delete records of Table and Catalog type |

## Module Schema

|**Name**|**Description**|
| :- | :- |
| Asset | New Fields has been added. Such as: Network, Subnet, Firmware, ESPZone, Facility, Zone, Level, Vendor, Asset Type, Protocol, Assets, Vulnerability Risk Status, Asset Change Activity, Asset Icon. Change In List View, Details View |
| Asset Resources | A Module that contain the Icons of Assets |
| Asset Change Activity | A module that monitors asset changes on various baselines. |
| Alert | Change in Details View |
| Incident | Change in Details View |

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

## Record Set

|**Name**|**Description**|
| :- | :- |
|  OT - Stuxnet Attack Scenario  |  This scenario recreates the Stuxnet attack in form of series of point alerts received by FortiSOAR from FortISIEM. |
| OT - Asset Change Activity | This scenario demonstrates the OT specific Asset Change Activity and Asset record creation process, which generates an Asset Change Activity and an Asset for type "Add New Asset" and "Medium Impact Baseline Change" activities. |

## Playbook Collection

|Playbook Collection Name |
| :- | 
| 00 - Use Case - Asset Change Activity |
| 00 - Use Case - Asset Management |

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
| Scenario - OT - Stuxnet Attack Scenario | Generate Alert for Stuxnet worm that targets Siemens S7 PLCs connected to Engineering Stations |
| Read CSV File | Playbook will read a CSV file and create records based on the record type. |
| Create Assets Record | This will generate an Asset record. |
| Create Assets Record | This will generate an Alert record. |
| Alert - Escalate To Incident | Creates a new incident with the given inputs and links the alert(s) to the newly created Incident. |
| Alert - Escalate To Incident (No Trigger) | Creates a new incident with the given inputs and links the alert(s) to the newly created Incident. |
| Alert - Escalate to Incident (Link Relations) | This playbook will extract related records and assign to incident created |
| Quarantine Asset and Raise Ticket | This playbook quarantine assets and raise ticket. |
| Isolate and Comment Assets | This PB will update the assets as isolate and add a comment. |
| Find Assets | Finds the asset based on the IP address provided. |
| On Alert Creation | Based on the MITRE Technique used for Alert, link the Sub Technique, Mitigation, Software, and Group. |



## System View
|**Name**|
| :- |
| Navigation Structure - Resources |


>**Warning:** We recommend that you clone these playbooks before customizing to avoid loss of information while upgrading the solution pack.
