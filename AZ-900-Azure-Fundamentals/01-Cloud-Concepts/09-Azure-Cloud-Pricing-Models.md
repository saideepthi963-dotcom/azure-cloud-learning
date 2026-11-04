# Azure Cloud Pricing Models

Azure offers different pricing options to help organizations balance **cost, flexibility, and long-term savings**.

The three main pricing models covered in this lecture are:

1. Pay-As-You-Go
2. Reserved Instances
3. Spot Pricing

## 1. Pay-As-You-Go

**Pay-As-You-Go means paying for Azure resources based on usage, without a long-term commitment.**

- No long-term commitment.
- Pay for the resources consumed.
- Easily increase or decrease resources.
- Generally higher per-unit cost than discounted pricing options.

**Best For:**
- Development and testing
- Short-term projects
- Workloads with unpredictable demand

**Remember:** Pay-As-You-Go = Maximum flexibility without a long-term commitment.

## 2. Reserved Instances (Reserved Capacity)

**Reserved Instances provide discounted pricing when you commit to eligible Azure resources for 1 or 3 years.**

- Commit for **1 year or 3 years**.
- Save up to **72%** compared with pay-as-you-go VM pricing in eligible scenarios.
- Best for resources used continuously.
- Less flexible than pay-as-you-go.

**Best For:**
- Production databases
- Applications running continuously
- Virtual desktop environments

**Remember:** Reserved Instances = Long-term commitment for lower costs.

## 3. Spot Pricing (Azure Spot VMs)

**Spot VMs allow you to use Azure's unused computing capacity at a discounted price.**

- Save up to **90%** compared with regular pay-as-you-go VM pricing.
- Uses unused Azure computing capacity.
- Azure can take back that capacity when needed.
- The VM may be **evicted (stopped or deleted)** with little warning.

**Best For:**
- Batch processing jobs
- Large-scale rendering
- Development and testing
- Applications that can handle interruptions

**Not suitable for:** Critical workloads that must run continuously without interruption.

**Remember:** Spot VMs = Very low cost, but risk of interruption.

## 4. Other Azure Pricing Options

**Enterprise Agreements**
- Designed for qualifying large organizations.
- May provide volume discounts and additional benefits.

**Azure Free Account**
- Offers eligible free services and introductory credits.
- Useful for beginners learning Azure.

**Dev/Test Offers**
- Provide eligible developers with discounted rates or special pricing for development and testing.

## 5. Comparison of Azure Pricing Models

| Feature | Pay-As-You-Go | Reserved Instances | Spot VMs |
|---|---|---|---|
| Commitment | None | 1 or 3 years | None |
| Cost | Regular rates | Discounted rates | Deep discounts |
| Flexibility | High | Lower | High, but interruptible |
| Interruption Risk | No Spot eviction risk | No Spot eviction risk | Can be evicted |
| Best For | Unpredictable workloads | Predictable, continuous workloads | Interruptible workloads |

## ⭐ Important AZ-900 Exam Points

- **Pay-As-You-Go:** Best for flexibility and unpredictable workloads.
- **Reserved Instances:** Best for predictable, long-running workloads.
- **Spot VMs:** Best for workloads that can tolerate interruptions.
- **Reserved Instances:** Can save up to 72% on eligible VM costs.
- **Spot VMs:** Can save up to 90% on eligible VM costs.
- **Eviction:** Azure can reclaim Spot VM capacity, interrupting the workload.
- **Pricing choice:** Depends on workload requirements, budget, and flexibility.

### Easy Way to Remember

**Pay-As-You-Go → Use whenever needed.**

**Reserved Instances → Commit longer, save money.**

**Spot VMs → Save more, but risk interruption.**