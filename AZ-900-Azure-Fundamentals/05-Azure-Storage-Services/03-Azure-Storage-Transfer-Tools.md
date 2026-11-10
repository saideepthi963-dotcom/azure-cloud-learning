# Azure Storage Transfer Tools

Azure provides tools to transfer and manage files stored in Azure Storage.

## 1. AzCopy

**AzCopy** is a command-line tool used to copy data to, from, or between Azure Storage locations.

Imagine your company has 1,000 files on a local computer and wants to upload them to Azure Blob Storage.

Instead of uploading each file manually, you can use AzCopy to transfer them efficiently.

AzCopy can run directly from the command line or in automation scripts.

Depending on the storage service and operation, it supports authentication using Microsoft Entra ID or a Shared Access Signature (SAS).

**Remember:** AzCopy → Transfer storage data using commands.

## 2. Azure Storage Explorer

**Azure Storage Explorer** is a desktop application that lets you view and manage Azure Storage using a graphical interface.

Think of it like File Explorer on your computer, but for Azure Storage.

You can upload, download, and manage storage data without writing commands.

It supports Windows, macOS, and Linux and works with Blob Storage, Azure Files, Queues, Tables, and Data Lake Storage Gen2.

**Remember:** Storage Explorer → Manage Azure Storage using a graphical application.

## 3. What Is a SAS Token?

A **Shared Access Signature (SAS)** gives limited access to Azure Storage resources without sharing the storage account key.

For example, you can allow someone to download a particular file for a limited time.

## 4. AzCopy vs. Storage Explorer

| AzCopy | Storage Explorer |
|---|---|
| Command-line tool | Graphical desktop application |
| Suitable for automated or large data transfers | Suitable for browsing and managing storage |
| Uses commands and scripts | Uses menus and buttons |

**Main takeaway:** AzCopy is useful for command-line file transfers, while Storage Explorer provides an easier visual way to manage Azure Storage data.