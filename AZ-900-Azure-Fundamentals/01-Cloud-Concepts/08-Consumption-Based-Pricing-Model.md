# Consumption-Based Pricing Model in Azure

## 1. What Is the Consumption-Based Model?

The **Consumption-Based Model** is a cloud pricing approach where organizations pay based on the resources they use.

Instead of purchasing expensive hardware upfront, organizations use Azure services and pay according to their usage.

**Simple meaning: Pay for what you use, like an electricity or water bill.**

## 2. Traditional IT vs. Cloud Computing

| Traditional IT (On-Premises) | Cloud Computing |
|---|---|
| Purchase physical hardware | Rent cloud resources |
| Large upfront costs | Usage-based costs |
| Maintain servers and equipment | Microsoft maintains physical infrastructure |
| Purchase capacity in advance | Adjust resources based on demand |
| Unused hardware still costs money | Reduce costs by removing unnecessary resources |

### Capital Expenditure (CapEx) vs. Operational Expenditure (OpEx)

- **CapEx (Capital Expenditure):** Money spent upfront to purchase assets such as servers, networking equipment, and datacenter infrastructure.
- **OpEx (Operational Expenditure):** Ongoing expenses for using and operating services, such as monthly cloud charges.

**Remember: Traditional IT often involves higher CapEx, while cloud computing shifts more spending toward OpEx.**

## 3. How Does Consumption-Based Pricing Work?

Azure **meters** resource usage, meaning it measures how much of a service you consume.

Examples:

- **Virtual Machines:** Charges can depend on how long a VM runs and its size.
- **Storage:** Charges depend on factors such as the amount and type of data stored.
- **Databases:** Charges depend on the selected service and pricing configuration.
- **Networking:** Certain data transfers and networking services generate usage-based charges.

**Important:** Stopping a resource doesn't always stop every charge. For example, a stopped VM may still incur storage charges.

## 4. Benefits of Consumption-Based Pricing

- **Lower upfront investment:** No need to purchase physical servers.
- **Pay-as-you-go:** Pay based on resource consumption.
- **Better cash flow:** Replace large hardware purchases with ongoing operating expenses.
- **Less waste:** Reduce unused computing capacity.
- **Flexibility:** Increase or decrease resources based on demand.
- **Cost visibility:** Monitor, analyze, and optimize spending using Azure cost management tools.

## 5. Example: Azure App Service

Imagine a website hosted using Azure App Service.

- **Normal traffic:** Runs using 2 application instances.
- **High traffic:** Scales out to 4 instances.
- **Traffic decreases:** Scales back in to 2 instances.

The organization pays for the additional provisioned capacity during the busy period, according to its App Service pricing plan.

**Key Point:** Scaling resources according to demand can improve performance while controlling costs.

## ⭐ Important AZ-900 Exam Points

- **Consumption-Based Model:** Pay based on resource usage.
- **CapEx:** Upfront spending on infrastructure.
- **OpEx:** Ongoing operating expenses.
- **Metering:** Measuring resource usage for billing.
- **Pay-as-you-go:** No long-term commitment is required for many Azure services.
- **Cost Optimization:** Adjust resources to reduce unnecessary spending.
- **Billing depends on the service:** Some resources continue generating charges even when they are not actively being used.

**Remember:**

**CapEx → Buy infrastructure.**

**OpEx → Pay ongoing expenses.**

**Consumption-Based Pricing → Pay according to Azure resource usage.**