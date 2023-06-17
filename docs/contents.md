| [Home](../README.md) |
| -------------------- |

# Contents

The **OT - Asset Management** solution pack contains the following resources.

## Dashboards

| Name                           | Description                                                                                                                |
| :----------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| Asset Change Activity Tracking | Track the activity over asset change                                                                                       |
| Asset Overview                 | This dashboard displays Assets By Level, By Zone, By Vendor By Category, By Level By State, By Type, By Vendor, By MEF Tag |
| Asset Risk Overview            | Displays the alerts over assets By Zone, By Criticality, and Recent Alerts                                                 |

## Connectors

| Name                | Version        | Description                                                                                                                                                                                                                                                |
| :------------------ | :------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| CSV Data Management | 1.2.0 or later | CSV Data management can perform different operations on CSV files like reading files, performing deduplication, merging two CSV files, joining two CSV files, concatenation of two CSV files, and returning a well-formatted dataset                       |
| Fortinet FortiEDR   | 1.3.0 or later | FortiEDR protects endpoints pre and post-infection, stopping data breaches in real-time and automatically orchestrating incident investigation and response. This connector facilitates automated operations related to events, forensics, and collectors. |
| Fortinet FortiGate  | 5.2.1 or later | Fortinet FortiGate enterprise firewall provides high performance, consolidated advanced security, and granular visibility for broad protection across the entire digital attack surface.                                                                   |
| ServiceNow          | 3.2.0 or later | ServiceNow connector provides functionality to create, read, update, and delete records of Table and Catalog type                                                                                                                                          |
| Qualys              | 1.0.1 or later | Qualys provides cloud security, compliance, and protection of IT assets and web applications. This connector facilitates automated operations for vulnerability management, policy compliance, and asset management.                                       |

## Widgets

| Name                | Description                                                                                                                                                                                                                                                                                                         |
| :------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Record Distribution | Ability to visualize items/records and their correlations in different levels based on a given grouping context. A very good example of the widget's utility is the OT view, where assets are visualized across different Purdue Levels and highlight any existing relations with other assets at different levels. |
 
## Module Schema

| Name                  | Description                                                |
| :-------------------- | :--------------------------------------------------------- |
| Asset                 | New field `Asset Icon`.                                    |
| Asset Resources       | A Module that contains the icons of assets                 |
| Asset Change Activity | A module that monitors asset changes on various baselines. |

## Picklist

| Name            |
| :-------------- |
| ActivityStatus  |
| AssetChangeType |
| AssetCategory   |

## Report

| Name                                 | Description                                   |
| :----------------------------------- | :-------------------------------------------- |
| Asset Change Activity Summary Report | Provide the report over asset change activity |


## Roles

| Name                 | Description                                                                       |
| :------------------- | :-------------------------------------------------------------------------------- |
| Full App Permissions | Full App Permissions for module **Asset Resources** and **Asset Change Activity** |

## Scenario Record Set

| Name                                         | Description                                                                                                                                                         |
| :------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| OT - Add Sample Assets                       | This scenario adds 86 different samples of OT Assets (different Purdue Levels, Types, etc.) for testing dashboards, use case playbooks, reports, and other actions. |
| OT - Add Sample Alerts                       | This scenario adds 12 well-populated samples OT Alerts for testing dashboards, use case playbooks, reports, and other actions.                                      |
| OT - Stuxnet Attack Scenario                 | This scenario recreates the Stuxnet attack in form of a series of point alerts received by FortiSOAR from FortISIEM.                                                |
| OT - Add Sample Asset Change Activity Record | This scenario generates a sample Asset Change Activity record each, for type "Add New Asset" and "Medium Impact Baseline Change" type of activities.                |

## Asset Resources Record Set

| Name                      | Description                                                          |
| :------------------------ | :------------------------------------------------------------------- |
| PLC                       | This contains the image file for the PLC icon.                       |
| WorkStation               | This contains the image file for the WorkStation icon.               |
| Laptop, Desktop, Endpoint | This contains the image file for Laptop, Desktop, and Endpoint icon. |
| Switch                    | This contains the image file for the Switch icon.                    |
| Server                    | This contains the image file for the Server icon.                    |
| Network                   | This contains the image file for the Network icon.                   |
| Router                    | This contains the image file for the Router icon.                    |
| HMI                       | This contains the image file for the HMI icon.                       |
| Firewall                  | This contains the image file for the Firewall icon.                  |
| Storage<sup>New<sup>      | This contains the image file for the Storage icon.                   |
| VOIP Phone<sup>New<sup>   | This contains the image file for the VOIP Phone icon.                |
| Gateway<sup>New<sup>      | This contains the image file for the Gateway icon.                   |
| Controller<sup>New<sup>   | This contains the image file for the Controller icon.                |
| Historian<sup>New<sup>    | This contains the image file for the Historian icon.                 |
| Printer<sup>New<sup>      | This contains the image file for the Printer icon.                   |

## Playbook Collection

### 08 - Utility - Asset Resources Management<sup>New<sup>

| Playbook Name                                               | Description                                                                                                                          |
| :---------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------- |
| Set VOIP Phone's Asset Icon<sup>New<sup>                    | Playbook attach the Workstation Icon from the Asset Resources to the Asset for the VOIP Phone                                        |
| Category.                                                   |
| Set Workstation's Asset Icon<sup>New<sup>                   | Playbook attach the Workstation Icon from the Asset Resources to the Asset for the Workstation Category.                             |
| Set Switch's Asset Icon<sup>New<sup>                        | Playbook attach the Switch Icon from the Asset Resources to the Asset for the Switch Category.                                       |
| Set Storage's Asset Icon<sup>New<sup>                       | Playbook attach the Storage Icon from the Asset Resources to the Asset for the Storage Category.                                     |
| Set Server's Asset Icon<sup>New<sup>                        | Playbook attach the Server Icon from the Asset Resources to the Asset for the Server Category.                                       |
| Set Router's Asset Icon<sup>New<sup>                        | Playbook attach the Router Icon from the Asset Resources to the Asset for the Router Category.                                       |
| Set Printer's Asset Icon<sup>New<sup>                       | Playbook attach the Printer Icon from the Asset Resources to the Asset for the Printer Category.                                     |
| Set PLC's Asset Icon<sup>New<sup>                           | Playbook attach the PLC Icon from the Asset Resources to the Asset for the PLC Category.                                             |
| Set Network's Asset Icon<sup>New<sup>                       | Playbook attach the Network Icon from the Asset Resources to the Asset for the Network Category.                                     |
| Set Laptop's, Desktop's, Endpoint's Asset Icon<sup>New<sup> | Playbook attach the Laptop, Desktop, Endpoint Icon from the Asset Resources to the Asset for the Laptop, Desktop, Endpoint Category. |
| Set Historian's Asset Icon<sup>New<sup>                     | Playbook attach the Historian Icon from the Asset Resources to the Asset for the Historian Category.                                 |
| Set HMI's Asset Icon<sup>New<sup>                           | Playbook attach the HMI Icon from the Asset Resources to the Asset for the HMI Category.                                             |
| Set Gateway's Asset Icon<sup>New<sup>                       | Playbook attach the Gateway Icon from the Asset Resources to the Asset for the Gateway Category.                                     |
| Set Firewall's Asset Icon<sup>New<sup>                      | Playbook attach the Firewall Icon from the Asset Resources to the Asset for the Firewall Category.                                   |
| Set Controller's Asset Icon<sup>New<sup>                    | Playbook attach the Firewall Icon from the Asset Resources to the Asset for the Controller Category.                                 |

### 02 - Use Case - Asset Change Activity

| Playbook Name                         | Description                                                                                        |
| :------------------------------------ | :------------------------------------------------------------------------------------------------- |
| Scenario - OT - Asset Change Activity | Generate an Asset Change Activity record for type Add New Asset and Medium Impact Baseline Change. |
| Medium Impact Baseline Change         | Baseline Change Workflow for Medium Impact Cyber Assets                                            |
| High Impact Baseline Change           | Baseline Change Workflow for High Impact Cyber Assets                                              |
| Add Cyber Asset                       | Baseline Change Workflow for Add Cyber Asset                                                       |
| Remove Cyber Asset                    | Baseline Change Workflow for Remove Cyber Asset                                                    |
| Replace Cyber Asset                   | Baseline Change Workflow for Replace Cyber Assets                                                  |
| Modify Cyber Asset                    | Baseline Change Workflow for Modify Cyber Asset                                                    |
| Add New Task                          | New task for Asset Change Activity                                                                 |
| Manage Asset Change Activity Closure  | Update the "Closed On" field with the current date and time if the status is Closed.               |
| Generate Asset Change Summary Report  | Generate report by manual trigger in FortiSOAR                                                     |
| Generate Report                       | Generates Report and Link to Incidents                                                             |

### 02 - Use Case - Asset Management

| Playbook Name                           | Description                                                                                     |
| :-------------------------------------- | :---------------------------------------------------------------------------------------------- |
| Scenario - OT - Create Assets Record    | Playbook reads a CSV file and create Assets records.                                            |
| > Create Assets Record                  | This will generate an Alert record.                                                             |
| Tag as Most Essential Function (MEF)    | Playbook tags asset as Most Essential Function(MEF)                                             |
| Scenario - OT - Create Alerts Record    | Playbook reads CSV file and create Alerts records.                                              |
| Scenario - OT - Stuxnet Attack Scenario | Generate Alert for Stuxnet worm that targets Siemens S7 PLCs connected to Engineering Stations. |
| Links Assets To Alert                   | Playbook correlates Assets on the basis of Source and Destination IP found in Alert.            |
| Find Assets Related To Alert            | Finds the asset based on the IP address provided.                                               |
| Quarantine Asset and Raise Ticket       | Playbook quarantine assets in FortiEDR and raise ticket in Service Now.                         |
| Isolate and Comment Assets              | Playbook update the assets as Isolate and add a comment.                                        |
| Update Firewall Policy                  | Update Firewall Policies To Restrict Communications.                                            |
| Scan All Assets Involved                | Initiate a quick scan on all assets related to the incident.                                    |
| Isolate Devices From Network            | Isolate Selected Devices From Network Based On Criticality and Risk.                            |

## System View
| Name                             |
| :------------------------------- |
| Navigation Structure - Resources |


>**Warning:** We recommend that you clone these playbooks before customizing to avoid loss of information while upgrading the solution pack.
