| [Home](../README.md) |
| -------------------- |

# Installation

1. To install a solution pack, click **Content Hub** > **Discover**.
2. Search and select **OT - Asset Management** from the list of solution pack that appears.
3. Click the **OT - Asset Management** solution pack card.
4. Click **Install** on the lower part of the screen to begin the installation.

## Prerequisites

The **OT - Asset Management** solution pack depends on the following solution packs that are installed automatically &ndash; if not already installed.

| Solution Pack Name                | Version         | Purpose                                                  |
| :-------------------------------- | :-------------- | :------------------------------------------------------- |
| SOAR Framework                    | v2.2.0 or later | Required for Alerts, Assets, Incident Response modules   |
| SOC Simulator                     | v1.0.1 or later | Required for Scenario Module and SOC Simulator connector |
| MITRE ATT&CK Enrichment Framework | v2.2.0 or later | Required for MITRE Modules and MITRE connector           |
| Vulnerability Management          | v2.1.0 or later | Required for Vulnerabilities and Scans Module            |

## After Installation

Ingest MITRE ATT&CK's **Group**, **Tactics**, **Techniques**, **Sub-techniques**, **Software**, and **Mitigation** data using the *MITRE ATT&CK* connector

<table>
    <tr>
        <td><strong>NOTE</strong></td>
        <td>On alert creation, IOCs are enriched, and the alerts are correlated with MITRE ATT&CK data for all records where the MITRE ATT&CK ID is associated with an alert.</td>
    </tr>
</table>

# Configuration

For optimal performance of the **OT - Asset Management** solution pack, you can install and configure the following connectors:

- **CSV Data Management** connectors to read CSV File. To configure and use the CSV Data Management connector, refer to [Configuring CSV Data Management](https://docs.fortinet.com/fortisoar/connectors/csvdatamngtnew)

- **Fortinet FortiEDR** connectors to Isolate collectors. To configure and use the Fortinet FortiEDR connector, refer to [Configuring Fortinet FortiEDR](https://docs.fortinet.com/fortisoar/connectors/fortiedr)

- **Fortinet FortiGate** connectors to Quarantine hosts, Update Policy. To configure and use the Fortinet FortiGate connector, refer to [Configuring Fortinet FortiGate](https://docs.fortinet.com/fortisoar/connectors/fortigate_firewall)

- **ServiceNow** connectors to raise tickets. To configure and use the ServiceNow connector, refer to [Configuring ServiceNow](https://docs.fortinet.com/fortisoar/connectors/servicenow-v2-0-1)

- **Qualys** connectors to get scanned host list. To configure and use the Qualys connector, refer to [Configuring Qualys](https://docs.fortinet.com/fortisoar/connectors/qualys)

| [Usage](./usage.md) | [Contents](./contents.md) |
|---------------------|---------------------------|