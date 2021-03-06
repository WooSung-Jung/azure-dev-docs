---
title: Manage storage accounts with Azure Explorer for Eclipse
description: Learn how to manage your Azure storage accounts by using the Azure Explorer for Eclipse.
documentationcenter: java
ms.date: 02/01/2018
ms.service: multiple
ms.tgt_pltfrm: multiple
ms.topic: article
---

# Manage storage accounts by using the Azure Explorer for Eclipse

The Azure Explorer, which is part of the Azure Toolkit for Eclipse, provides Java developers with an easy-to-use solution for managing storage accounts in their Azure account from inside the Eclipse integrated development environment (IDE).

[!INCLUDE [prerequisites](includes/prerequisites.md)]

[!INCLUDE [show-azure-explorer](includes/show-azure-explorer.md)]

## Create a storage account in Eclipse

To create a storage account by using the Azure Explorer, do the following:

1. Sign in to your Azure account by using the [Sign-in instructions for the Azure Toolkit for Eclipse](/azure/developer/java/toolkit-for-eclipse/sign-in-instructions).

1. In the **Azure Explorer** view, expand the **Azure** node, right-click **Storage Accounts**, and then click **Create Storage Account**.

   ![Create Storage Account command][CS01]

1. In the **Create Storage Account** dialog box, specify the following options:

   ![Create New Storage Account dialog box][CS02]

   * **Name**: Specifies the name for the new storage account.

   * **Subscription**: Specifies the Azure subscription that you want to use for the new storage account.

   * **Resource Group**: Specifies the resource group for your virtual machine. Select one of the following options:
      * **Create New**: Specifies that you want to create a new resource group.
      * **Use Existing**: Specifies that you will select from a list of resource groups that are associated with your Azure account.

   * **Region**: Specifies the location where your storage account will be created (for example, "West US").

   * **Account kind**: Specifies the type of storage account to create (for example, "Blob storage"). For more information, see [About Azure storage accounts].

   * **Performance**: Specifies which storage account offering to use from the selected publisher (for example, "Premium"). For more information, see [Azure storage scalability and performance targets].

   * **Replication**: Specifies the replication for the storage account (for example, "Zone-Redundant"). For more information, see [Azure storage replication].

1. When you have specified all of the preceding options, click **Create**.

## Create a storage container in Eclipse

To create a storage container by using the Azure Explorer, do the following:

1. In the **Azure Explorer** view, right-click the storage account where you want to create a container, and then click **Create blob container**.

   ![Create blob container command][CC01]

1. In the **Create blob container** dialog box, specify the name for your container, and then click **OK**. For more information about naming storage containers, see [Naming and referencing containers, blobs, and metadata].

   ![Create blob container dialog box][CC02]

## Delete a storage container in Eclipse

To delete a storage container by using the Azure Explorer, do the following:

1. In the **Azure Explorer** view, right-click the storage container, and then click **Delete**.

   ![Delete storage container command][DC01]

1. In the confirmation window, click **OK**.

   ![Delete storage container confirmation window][DC02]

## Delete a storage account in Eclipse

To delete a storage account by using the Azure Explorer, do the following:

1. In the **Azure Explorer** view, right-click the storage account, and then click **Delete**.

   ![Delete storage account command][DS01]

1. In the confirmation window, click **OK**.

   ![Delete storage account confirmation window][DS02]

## Next steps

For more information about Azure storage accounts, sizes, and pricing, see the following resources:

* [Introduction to Microsoft Azure Storage]
* [About Azure storage accounts]
* Azure storage-account sizes
  * [Sizes for Windows storage accounts in Azure]
  * [Sizes for Linux storage accounts in Azure]
* Azure storage-account pricing
  * [Windows storage-account pricing]
  * [Linux storage-account pricing]

[!INCLUDE [additional-resources](includes/additional-resources.md)]

<!-- URL List -->

[Introduction to Microsoft Azure Storage]: /azure/storage/common/storage-introduction
[About Azure storage accounts]: /azure/storage/storage-create-storage-account
[Azure storage replication]: /azure/storage/storage-redundancy
[Azure storage scalability and Performance Targets]: /azure/storage/storage-scalability-targets
[Naming and referencing containers, blobs, and metadata]: https://go.microsoft.com/fwlink/?LinkId=255555

[Sizes for Windows storage accounts in Azure]: /azure/virtual-machines/virtual-machines-windows-sizes
[Sizes for Linux storage accounts in Azure]: /azure/virtual-machines/virtual-machines-linux-sizes
[Windows storage-account pricing]: https://azure.microsoft.com/pricing/details/virtual-machines/windows/
[Linux storage-account pricing]: https://azure.microsoft.com/pricing/details/virtual-machines/linux/

<!-- IMG List -->

[CS01]: media/managing-storage-accounts-using-azure-explorer/CS01.png
[CS02]: media/managing-storage-accounts-using-azure-explorer/CS02.png
[CC01]: media/managing-storage-accounts-using-azure-explorer/CC01.png
[CC02]: media/managing-storage-accounts-using-azure-explorer/CC02.png

[DS01]: media/managing-storage-accounts-using-azure-explorer/DS01.png
[DS02]: media/managing-storage-accounts-using-azure-explorer/DS02.png
[DC01]: media/managing-storage-accounts-using-azure-explorer/DC01.png
[DC02]: media/managing-storage-accounts-using-azure-explorer/DC02.png
