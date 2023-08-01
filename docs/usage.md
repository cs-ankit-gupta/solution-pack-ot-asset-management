| [Home](../README.md) |
| -------------------- |

# Usage

Refer to [Simulate Scenario documentation](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/docs/usage.md) to understand how to simulate and reset scenarios.

To understand the process FortiSOAR&trade; follows to respond to **Asset Management**, **Baseline changes over assets**, and **Alerts over Assets**, we have included following scenarios with this solution pack:

- OT - Add Sample Assets

- OT - Add Sample Alerts

- OT - Stuxnet Attack Scenario

- OT - Asset Change Activity

Refer to the subsequent sections to understand how this solution pack's automation addresses your needs.

## Simulations

The simulation mode has some sample data that helps you get a better understanding of how the solution pack functions. Following steps help you use the solution pack with some included sample data.

### OT - Add Sample Assets

This scenario generates 86 OT Assets of different Levels, Types, and other categories as an example for testing dashboards, use case playbooks, reports and other actions.

To run this scenario and generate the alerts perform the following steps:

1. Under the FortiSOAR&trade; menu select to open **Simulations**.

2. Select the scenario **OT - Add Sample Assets**.

3. Click **Simulate Scenario**.

### OT - Add Sample Alerts

This scenario generates 12 well-populated OT Alerts as an example for testing dashboards, use-case playbooks, reports, and other actions.

To run this scenario and generate the alerts perform the following steps:

1. Under the FortiSOAR&trade; menu select to open **Simulations**.

2. Select the scenario **OT - Add Sample Alerts**.

3. Click **Simulate Scenario**.

### OT - Stuxnet Attack Scenario

This scenario generates following alerts, each at an interval of 2 seconds:

- Stuxnet peer-to-peer communication attempt
- Anomalous communication between two Windows XP machines
- Communication between public and private networks
- STEP7 configuration download command

<table>
    <tr>
        <td><strong>IMPORTANT</strong></td>
        <td>Ensure that the global variable <code>Demo mode</code> is set to <code>true</code>.</td>
    </tr>
</table>

Navigate to the newly-created alerts and observe the following:

- Each asset is created and added to the record with the following hostname:

    - PLC S7-400-324
    - Dell - 5490-42E6
    - ThinkCentre M910s-1181
    - HP - PB7181

- Each alert is associated with assets based on the assets' source and destination IP.

- The **Correlations** tab of an alert links *Group*, *Tactics*, *Technique*, *Sub-Technique*, and *Software*.

- Possible mitigation actions are listed in the alert's **Recommended ATT&CK Mitigation** tab.

- After enrichment completes, the **Stuxnet peer-to-peer communication attempt** alert contains similar alerts in the **Workspace** > **Recommendations** tab. 

    - You can escalate this alert to an incident by selecting **Select All** and **Include this record** checkboxes, click the **Playbook** drop-down and select **Escalate**.
    
    - On the **Escalate** pop-up window, enter relevant details and click the button **Escalate**. An incident is created with the link available in the alert's comment.

- Incidents are correlated with all the *Indicators*, *Alerts*, *Assets*, *Technique*, *Mitigation*, and *Software*.

- Click on **Quarantine Asset and Raise Ticket** to quarantine assets and raise ticket for assets.

- You can generate report by using **Generate Incident Summary Report**

- Use the **Setup War Room** button to create a war room. All of the alerts, incidents, affected assets, and IOCs will be in the war room.

- Playbooks in the War Room can be used to take action, such as `Isolate Devices From Network`, `Scan All Assets Involved`, and `Update Firewall Policy`.

To run this scenario and generate the alerts perform the following steps:

1. Under the FortiSOAR&trade; menu select to open **Simulations**.

2. Select the scenario **OT - Stuxnet Attack**.

3. Click **Simulate Scenario**.

### OT - Add Sample Asset Change Activity Record

- Browse to **Simulations** > **OT - Add Sample Asset Change Activity Record** scenario and click **Simulate Scenario**.

    <table>
        <tr>
            <td><strong>NOTE</strong></td>
            <td><strong>Scenario - OT - Asset Change Activity</strong> has a variable <code>dueDays</code> (<em>Days required to complete change activity</em>). You can populate these variables with your preferred values in the <em>Configuration</em> step.</td>
        </tr>
    </table>

- With a given value of due date in `dueDays` two Asset Change Activity entries are made.
    - Add New Cyber Asset - Siemens S7-400-S621
    - Medium Impact Baseline Change - Stratix 5950-RW41

- Assets are linked and can be seen in the Assets & Vulnerabilities tab.

- Once the record has been created, execute the **Add Task From Templates** to assign different tasks to different people. 

- New tasks get created as priority **Medium** once the previous task is completed.

- New task can be added by using **Add New Task** playbook.

- Once all task get completed record get closed.

- To generate the report, execute **Generate Compliance Report** and report get attached to particular record comments.

| [Installation](./setup.md#installation) | [Configuration](./setup.md#configuration) | [Contents](./contents.md) |
|-----------------------------------------|-------------------------------------------|---------------------------|