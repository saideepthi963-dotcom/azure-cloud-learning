# Azure Monitoring and Reporting

## 1. Azure Resource Tags

**Tags** help organize Azure resources using a name and value.

For example, a company can label its resources:

- `Environment = Production`
- `Environment = Development`
- `Department = Finance`

Tags help with **resource organization, management, and cost tracking**, even across resource groups.

**Important:** Tags applied to a resource group are not automatically inherited by its resources. Azure Policy can help enforce tagging rules.

## 2. Azure Monitor

**Azure Monitor** collects and analyzes monitoring data to help identify problems with applications and Azure resources.

Imagine a company runs an application on an Azure VM. Azure Monitor can track CPU usage, detect performance issues, and send alerts.

It collects two important types of data:

- **Metrics:** Numerical performance measurements, such as CPU usage.
- **Logs:** Records of events and activities, such as resource changes and errors.

Azure Monitor can collect data from applications, operating systems, Azure resources, subscriptions, and tenant services.

## 3. Azure Service Health

**Azure Service Health** helps organizations understand Azure service issues, planned maintenance, and resource availability.

| Service | What It Shows |
|---|---|
| **Azure Status** | Global health of Azure services |
| **Service Health** | Azure service issues and maintenance affecting your subscriptions |
| **Resource Health** | Health and availability of your individual Azure resources |

**Example:** If your Azure VM becomes unavailable, Resource Health can help determine whether an Azure platform issue affected it.

## 4. Azure Monitor Insights

Azure Monitor provides specialized monitoring capabilities.

| Feature | What It Monitors |
|---|---|
| **Application Insights** | Application performance, usage, and errors |
| **VM Insights** | Virtual machine performance and health |
| **Container Insights** | Kubernetes container performance and logs |

## 5. Azure Monitor Actions

Azure Monitor helps you respond to monitoring data through:

- **Alerts:** Notify administrators when a problem occurs.
- **Autoscale:** Automatically adjust supported resources based on workload.
- **Dashboards and Charts:** Visualize monitoring data.
- **Integrations:** Connect monitoring data with other services and tools.

## Key Takeaway

| Azure Feature | Remember |
|---|---|
| **Tags** | Organize resources |
| **Azure Monitor** | Monitor performance, metrics, and logs |
| **Azure Status** | Global Azure service health |
| **Service Health** | Azure issues affecting your subscriptions |
| **Resource Health** | Health of individual resources |
| **Application Insights** | Monitor application performance |
| **VM Insights** | Monitor virtual machines |
| **Container Insights** | Monitor Kubernetes containers |