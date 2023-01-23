| [Home](../README.md) |
|--------------------------------------------|

# Installation

1. To install a solution pack, click **Content Hub** > **Discover**.
2. From the list of solution pack that appears, search for and select `OT - Asset Management`.
3. Click the `OT - Asset Management` solution pack card.
4. Click **Install** on the bottom to begin installation.

## Prerequisites

The `OT - Asset Management` solution pack depends on the following solution packs that are installed automatically &ndash; if not already installed.

| **Solution Pack Name** | **Version** | **Purpose**   |
| :--------------------- | :---------------------| :--------------------------------------- |
| SOAR Framework | v2.0.1 or later | Required for Alerts, Assets, Incident Response modules | 
| SOC Simulator | v1.0.1 or later | Required for Scenario Module and SOC Simulator connector |
| MITRE ATT&CK Enrichment Framework | v2.0.3 or later | Required for MITRE Modules and MITRE connector |
| Vulnerability Management | v2.0.0 or later | Required for Vulnerabilities and Scans Module |


# Configuration

For optimal performance of `OT - Asset Management` solution pack, you can install and configure the connectors that help with the following:

>**Example**:
>* **Fortinet FortiEDR** connectors to Isolate collectors. To configure and use the Fortinet FortiEDR connector, refer to [Configuring Fortinet FortiEDR](https://docs.fortinet.com/document/fortisoar/1.3.0/fortinet-fortiedr/161/fortinet-fortiedr-v1-3-0)
>* **ServiceNow** connectors to raise tickets. To configure and use the ServiceNow connector, refer to [Configuring ServiceNow](https://docs.fortinet.com/document/fortisoar/3.2.0/servicenow/384/servicenow-v3-2-0)