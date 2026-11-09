# Azure Management Tools

Azure provides different tools to manage cloud resources. Some use a graphical interface, while others use commands or code to automate tasks.

## 1. Azure Portal

The **Azure Portal** is a website where you can create, manage, delete, and monitor Azure resources using a graphical interface.

You don't need to write commands. You can simply navigate through menus and select options.

**Best for:** Beginners and everyday resource management.

## 2. Azure PowerShell vs. Azure CLI

Both tools let you manage Azure resources by typing commands instead of clicking through the portal.

| Azure PowerShell | Azure CLI |
|---|---|
| Uses PowerShell commands | Uses `az` commands |
| Common in PowerShell automation | Common in cross-platform automation |
| Example: `New-AzVM` | Example: `az vm create` |

Both support Windows, Linux, and macOS.

**Why use them?** Imagine you need to create 50 virtual machines. Instead of manually repeating the process in the portal, you can automate it using scripts.

## 3. Azure Cloud Shell

**Azure Cloud Shell** lets you run Azure PowerShell or Azure CLI directly in your browser.

You don't need to install command-line tools on your computer.

You can choose:
- **Bash:** Uses Azure CLI commands.
- **PowerShell:** Uses Azure PowerShell commands.

Cloud Shell provides options for temporary sessions or persistent file storage.

**Remember:** Cloud Shell = Browser-based command-line environment.

## 4. Azure Mobile App

The **Azure Mobile App** lets you monitor and manage Azure resources using your phone.

You can check alerts, monitor resource health, and perform common tasks such as restarting virtual machines.

**Best for:** Managing Azure resources while away from your computer.

## 5. Azure REST APIs

**Azure REST APIs** allow applications to communicate with Azure over HTTP.

For example, a developer can write a program that sends requests to Azure to create or manage resources.

Common HTTP operations include:

- `GET` → Retrieve information.
- `POST` → Send requests or create resources.
- `PUT` → Create or update resources.
- `DELETE` → Delete resources.

**Remember:** REST APIs = Manage Azure programmatically through HTTP requests.

## 6. Azure Advisor

**Azure Advisor** analyzes your Azure environment and recommends improvements.

It helps identify ways to reduce costs, improve performance, strengthen security, and increase reliability.

For example, if a VM is underutilized, Advisor might recommend resizing it to save money.

**Remember:** Azure Advisor = Personalized recommendations to improve Azure resources.

---

## ⭐ AZ-900 Exam: Which Tool Should You Choose?

| Question Mentions | Choose |
|---|---|
| Manage Azure through a website | **Azure Portal** |
| Automate using PowerShell commands | **Azure PowerShell** |
| Run `az` commands | **Azure CLI** |
| Run commands directly in a browser | **Azure Cloud Shell** |
| Manage resources from a phone | **Azure Mobile App** |
| Manage Azure through HTTP requests | **Azure REST APIs** |
| Get cost, security, performance, or reliability recommendations | **Azure Advisor** |

**Main takeaway:** Azure offers graphical, command-line, mobile, and programming interfaces for managing resources, while Azure Advisor helps you improve your environment.

## 7. Azure Arc

**Azure Arc** allows you to manage resources outside Azure using Azure's management tools.

Imagine a company has servers in three different places:

- **On-premises:** Servers in its own datacenter.
- **Azure Cloud:** Resources running in Azure.
- **AWS:** Resources running in another cloud provider.

Instead of managing everything separately, **Azure Arc connects supported resources to Azure so they can be managed from one place.**

### What Can Azure Arc Do?

**Unified Management:** Manage supported resources across on-premises, Azure, other clouds, and edge locations.

**Consistent Governance:** Apply Azure policies, security controls, and compliance rules across connected environments.

**Azure Services Anywhere:** Extend supported Azure capabilities and services to infrastructure outside Azure.

**Hybrid and Multi-Cloud Support:** Helps organizations manage resources across different computing environments.

### ⭐ AZ-900 Exam Tip

**Azure Arc → Manage resources outside Azure using Azure management tools.**

Remember:

**Azure Portal → Manage Azure resources through a browser.**

**Azure Advisor → Get recommendations to improve Azure resources.**

**Azure Arc → Extend Azure management to on-premises and other clouds.**

## 8. Creating a Virtual Machine Using Azure PowerShell

Azure PowerShell allows you to create and manage Azure resources by running commands instead of using the Azure Portal's graphical interface.

### Example: Create an Ubuntu Virtual Machine

Open **Azure Cloud Shell**, select **PowerShell**, and run:

```powershell
New-AzVM `
    -ResourceGroupName "myresourcegroup" `
    -Name "MyVM-01" `
    -Image "Ubuntu2204"
```

### Understanding the Command

| Parameter | Purpose |
|---|---|
| `New-AzVM` | Creates a new Azure Virtual Machine |
| `-ResourceGroupName` | Specifies which resource group will contain the VM |
| `-Name` | Specifies the VM's name |
| `-Image` | Specifies the operating system image |

In this example, we're creating a VM named `MyVM-01` running Ubuntu Linux.

If you don't specify networking information, `New-AzVM` can automatically create supporting resources such as a virtual network, subnet, network interface, and public IP address.

The command may also prompt you to provide VM login credentials.

### ⭐ AZ-900 Exam Tip

**Azure PowerShell → Manage Azure resources using PowerShell commands.**

**Azure Cloud Shell → Run PowerShell or Azure CLI directly in a browser.**

**`New-AzVM` → Creates an Azure Virtual Machine.**

You don't need to memorize the entire command for AZ-900. Focus on understanding what each management tool does.