# Azure Compute Services

## 1. What Is Azure Compute?

**Azure Compute** provides the computing power needed to run applications in the cloud.

Instead of purchasing physical servers, you can use Azure's processors (CPU), memory (RAM), storage, and networking resources whenever you need them.

Resources are available on demand, and costs depend on the service and how much you use it.

Azure supports different operating systems and enterprise workloads, including Windows, Linux, SQL Server, Oracle, and SAP.

## 2. Azure Virtual Machines (VMs)

An **Azure Virtual Machine** is like having your own computer or server in the cloud.

It has a CPU, memory, storage, networking, and an operating system.

You can install software, configure the operating system, and remotely access the machine.

**When to use:** When you need full control over the operating system and installed software.

**Service Model:** Infrastructure as a Service (IaaS).

## 3. Virtual Machine Scale Sets (VMSS)

Imagine your website normally needs 2 VMs, but during a busy period, it needs 10.

Instead of manually creating more VMs, **Virtual Machine Scale Sets** help you manage multiple similarly configured VMs and scale their number based on demand.

- More traffic → Add VMs.
- Less traffic → Remove VMs.

Scaling can be automatic or manual.

**When to use:** Applications that need multiple VMs and flexible scaling.

## 4. Azure Container Instances (ACI) and Azure Kubernetes Service (AKS)

A **container** is a lightweight package containing an application and the components it needs to run.

Unlike a VM, a container doesn't require its own complete operating system. Containers share the host operating system's kernel.

Azure provides two important container services:

**Azure Container Instances (ACI):** Run containers without managing servers or a container orchestration platform.

**Azure Kubernetes Service (AKS):** Deploy and manage containerized applications using Kubernetes, especially when running many containers together.

**Remember:** ACI is simpler for running containers, while AKS provides more advanced container management.

## 5. Azure App Service

**Azure App Service** is a fully managed platform for hosting web applications and APIs.

You focus on building and deploying your application, while Azure manages the underlying infrastructure.

**When to use:** Hosting websites, web applications, and APIs without managing servers.

**Service Model:** Platform as a Service (PaaS).

## 6. Azure Functions

**Azure Functions** lets you run code in response to an event without managing the underlying servers.

An event could be:
- An HTTP request.
- A scheduled timer.
- A message from another Azure service.

**Example:** Automatically run code when a new file is uploaded.

This approach is called **serverless computing**.

Serverless doesn't mean there are no servers. It means Azure manages them for you.

**When to use:** Running event-driven code without managing infrastructure.

*Note: Azure Functions also supports longer-running workflows; it's not limited to tasks lasting only a few seconds.*

---

## ⭐ Azure Compute Services — AZ-900 Comparison

| Azure Service | Main Purpose |
|---|---|
| **Virtual Machines** | Run software with control over the operating system |
| **VM Scale Sets** | Manage and scale multiple VMs |
| **Container Instances** | Run containers without managing servers |
| **Azure Kubernetes Service** | Manage and orchestrate containerized applications |
| **App Service** | Host web apps and APIs |
| **Azure Functions** | Run event-driven code without managing servers |

### 🎯 Easy Way to Remember

**Need your own cloud server?** → Virtual Machines

**Need multiple VMs that scale?** → VM Scale Sets

**Need to run a container?** → Container Instances

**Need to manage many containers?** → AKS

**Need to host a website?** → App Service

**Need to run code when something happens?** → Azure Functions


## 7. Serverless Computing

**Serverless Computing** means running applications without managing the underlying servers.

Servers still exist, but **Azure handles their maintenance, scaling, and infrastructure**. You focus on writing and deploying your code.

### How Does Serverless Work?

Imagine you want to automatically process a file whenever someone uploads it.

1. You write the code to process the file.
2. You deploy it to Azure.
3. When a file is uploaded, Azure runs your code.
4. Azure scales the resources based on demand.

This is called **event-driven computing** because an event triggers the application.

### Azure Serverless Services

| Service | What It Does |
|---|---|
| **Azure Functions** | Runs code when an event occurs. |
| **Azure Logic Apps** | Automates workflows with little or no code. |
| **Azure Event Grid** | Routes events between Azure services and applications. |
| **Azure Container Apps** | Runs containerized applications without managing Kubernetes infrastructure. |

### Why Use Serverless?

Serverless reduces infrastructure management and automatically scales based on demand.

It is useful for processing file uploads, scheduling tasks, automating workflows, and handling incoming events.

**Cost:** Some serverless plans charge based on actual executions and resource consumption rather than continuously running servers. Pricing depends on the service and plan.

### ⭐ AZ-900 Exam Tips

**Serverless →** Azure manages the infrastructure.

**Event-driven →** Code runs when a particular event occurs.

**Azure Functions →** Execute code.

**Azure Logic Apps →** Automate workflows.

**Azure Event Grid →** Route events.

**Azure Container Apps →** Run containers without managing Kubernetes.

**Remember:** Serverless doesn't mean there are no servers. It means you don't manage them.