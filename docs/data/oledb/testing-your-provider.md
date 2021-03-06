---
title: Testing Your Provider | Microsoft Docs
ms.custom: 
ms.date: 11/04/2016
ms.reviewer: 
ms.suite: 
ms.technology:
- devlang-cpp
ms.tgt_pltfrm: 
ms.topic: article
dev_langs:
- C++
helpviewer_keywords:
- testing, OLE DB providers
- testing providers
- OLE DB providers, testing
ms.assetid: bf824fe4-81af-4ffb-beb3-4fa2928dc450
caps.latest.revision: 11
author: mikeblome
ms.author: mblome
manager: ghogen
translation.priority.ht:
- cs-cz
- de-de
- es-es
- fr-fr
- it-it
- ja-jp
- ko-kr
- pl-pl
- pt-br
- ru-ru
- tr-tr
- zh-cn
- zh-tw
translationtype: Human Translation
ms.sourcegitcommit: 5187996fc377bca8633360082d07f7ec8a68ee57
ms.openlocfilehash: a3c62c9e5338bef58dec15d6550a4cd395d5dcb0

---
# Testing Your Provider
Before you release a provider, you should perform the following tests, in the order indicated. These tests ensure that the provider functions properly for most potential users.  
  
1.  Test the provider using a [consumer](../../data/oledb/creating-an-ole-db-consumer.md) application written with the OLE DB consumer templates. The test consumer should cover all functional areas of your provider (all code that you have added or modified).  
  
2.  Test the provider using a consumer application written with ADO. Most developers (especially Microsoft Visual Basic and Microsoft C# developers) use ADO or ADO.NET for consumer applications. The test consumer should cover all functional areas of your provider. For an example of an ADO consumer application, see [ADO Code Examples in Microsoft Visual Basic](https://msdn.microsoft.com/en-us/library/ms807514.aspx).  
  
3.  Run the OLE DB conformance tests (including ADO conformance tests) to ensure that your provider meets the level 0 standard for OLE DB providers. (For an explanation of level 0, search for "OLE DB Level 0 Conformance Tests" at [OLE DB Programmer's Guide](http://go.microsoft.com/fwlink/?linkid=121548). These tests and associated documentation are included with Visual C++ in the Data Access SDK. These tests also help to ensure that your provider runs well when aggregated by other [service providers](../../data/oledb/ole-db-resource-pooling-and-services.md) and are especially useful if you modify or add properties. For more information about the conformance tests, see the Readme file for the Data Access SDK, which is located on one of the Visual Studio CDs.  
  
## See Also  
 [Working with OLE DB Provider Templates](../../data/oledb/working-with-ole-db-provider-templates.md)


<!--HONumber=Jan17_HO2-->


