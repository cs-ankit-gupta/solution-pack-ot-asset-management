
| [Home](../README.md) |
|--------------------------------------------|

# Usage

Refer to [Simulate Scenario documentation](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/docs/solution-pack-guide.md) to understand how to simulate and reset scenarios.

To understand the process FortiSOAR follows to respond to **Asset Management**, **Baseline changes over assets** and **Alerts over Assets**, we have included a scenario &mdash; `OT - Asset Change Activity` and `OT - Stuxnet Attack Scenario` with this solution pack. 

Refer to the section `OT - Asset Management` to understand how this solution pack automation addresses your needs.

# OT- Asset Management

### Steps to be followed after installing SP:

1. Use Playbook - **MITRE ATT&CK > Fetch Latest Data** from MITRE Connector Sample Playbook to get the Tactics, Techniques, Sub-techniques, Mitigations, Groups and Software.
2. Import sample Assets by excuting Playbook **Read CSV File** over Attachment record `Asset_Record`
3. Import sample Alerts by excuting Playbook **Read CSV File** over Attachment record `Alert_Record`

> Note: On alert creation, IOCs are enriched, and the alert is correlated with Techniques, Mitigation, and all other records for the MITRE ATT&CK Id that is present in the alert.

## Simulation mode

The simulation mode has some sample data that helps you get a better understanding of how the solution pack functions. Following steps help you use the solution pack with some included sample data.

Please set Demo_mode **true**

> **1. OT - Stuxnet Attack Scenario**
-   Make sure the global variable **Demo mode** is set to `true`. 
- Browse to `Simulations` > `OT - Stuxnet Attack Scenario` scenario and click **Simulate Scenario**.
- Four Alerts are created each at an interval of 2 seconds:
    - Stuxnet peer to peer communication attempt
    - Anomalous communication between two Windows XP machines
    - Communication between public and private networks
    - STEP7 configuration download command
- Each alert get associated with assets based on the Source and Destination IP.
- **Technique**, **Mitigation** and **Software** get linked to alerts under the **Recommended Mitigation** tab.
- Once the alert has been enriched, open the "Stuxnet peer to peer communication attempt" alert and look for a similar alert in the Workspace Recommendations tab. 
- Escalate the alert to an incident by checking "Select All" and "Include this record," then running the playbook **Escalate To Incident**. Please provide all incident details. (An incident is created with the link available in the alert's comment)
- Incident get correlated with all the IOCs, Alerts, Assets, Technique, Mitigation and Software.
- Click on **Quarantine Asset and Raise Ticket** to quarantine assets and raise ticket for assets.
- You can generate report by using **Generate Incident Summary Report**

> **2. OT - Asset Change Activity**
- Browse to `Simulations` > `OT - Asset Change Activity` scenario and click **Simulate Scenario**.
- Playbook: **Scenario - OT - Asset Change Activity** has two variables `dueDays` and `mediumImpactAsset`. You can populate these variables with your preferred names in the *Configuration* step. 
    - `dueDays` - Days required to complete change activity.
    - `mediumImpactAsset` - Impacted Asset hostname.
- Two Asset Change Activity records are created with a due date of the next two days. 
    - Add New Cyber Asset - Intel Core i7-13700K
    - Medium Impact Baseline Change - Patch For log 4J
- Assets are linked and can be seen in the Assets & Vulnerabilities tab.
- Once the record has been created, execute the **Add Task From Templates** to assign different tasks to different people. 
- New tasks get created after the previous task is completed.
- Once all task get completed record get closed.

