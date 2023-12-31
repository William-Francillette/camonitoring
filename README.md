# Conditional Access Monitoring Automation
The Conditional Access Monitoring project is a proof-of-concept to monitor your Entra Conditional Access policy drift using **[Microsoft 365 DSC](https://microsoft365dsc.com/home/what-is-M365DSC/)** and **Sentinel**.

The deployment process is automated using Azure DevOps and the following pipeline:

*camonitoring-cd-m365dsc-with-public-ip.yml* provisions:
- Resource Group x1
- VM x1
- NIC x1
- Managed Disk x1
- vNet x1
- NSG x1
- Public IP x1
- Storage Account x1
- AMA extension 
- DCR Rule x1 
- DCR Association x1

## Pre exisisting resources
The following resources should already be configured:

- Log Analytics Workspace
- Sentinel Instance
- Sentinel Analytic rules

For more information, refer to the following blog post: [M365DSC: Monitor Conditional Access Policy Configuration Drift with Microsoft Sentinel](https://www.french365connection.co.uk/post/m365dsc-monitor-conditional-access-policy-configuration-drift-with-microsoft-sentinel#viewer-9vm7a)
