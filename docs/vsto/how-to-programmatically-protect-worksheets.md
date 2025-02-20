---
title: "Programmatically protect worksheets"
description: Learn how you can use the protection feature in Microsoft Excel to prevent users and code from modifying objects in a worksheet.
ms.date: "02/02/2017"
ms.topic: "how-to"
dev_langs:
  - "VB"
  - "CSharp"
helpviewer_keywords:
  - "protection, adding to worksheets"
  - "documents [Office development in Visual Studio], document protection"
  - "document protection, adding to worksheets"
  - "worksheets, protecting"
author: John-Hart
ms.author: johnhart
manager: jmartens
ms.subservice: office-development
---
# Programmatically protect worksheets

  The protection feature in Microsoft Office Excel helps prevent users and code from modifying objects in a worksheet. By default, all cells are locked after you turn on protection.

 [!INCLUDE[appliesto_xlalldocapp](../vsto/includes/appliesto-xlalldocapp-md.md)]

 In document-level customizations, you can protect worksheets by using the Excel designer. You can also protect a worksheet programmatically at run time in any project type.

> [!NOTE]
> You cannot add Windows Forms controls to areas of a worksheet that are protected.

## Use the designer

### To protect a worksheet in the designer

1. In the **Changes** group of the **Review** tab, click **Protect Sheet**.

    The **Protect Sheet** dialog box appears. You can set a password and optionally specify certain actions that users are allowed to perform with the worksheet, such as format cells or insert rows.

   You can also allow users to edit specific ranges in protected worksheets.

### To allow editing in specific ranges

1. In the **Changes** group of the **Review** tab, click **Allow Users to Edit Ranges**.

     The **Allow Users to Edit Ranges** dialog box appears. You can specify ranges that are unlocked using a password, and users who can edit ranges without a password.

## Use code at run time
 The following code sets the password (using the variable getPasswordFromUser, which contains a password obtained from the user) and allows only sorting.

### To protect a worksheet by using code in a document-level customization

1. Call the <xref:Microsoft.Office.Tools.Excel.Worksheet.Protect%2A> method of the worksheet. This example assumes that you are working with a worksheet named `Sheet1`.

     ### [C#](#tab/csharp)
     :::code language="csharp" source="../vsto/codesnippet/CSharp/Trin_VstcoreExcelAutomationCS/Sheet1.cs" id="Snippet27":::

     ### [VB](#tab/vb)
     :::code language="vb" source="../vsto/codesnippet/VisualBasic/Trin_VstcoreExcelAutomation/Sheet1.vb" id="Snippet27":::
     ---

### To protect a worksheet by using code in a VSTO Add-in

1. Call the <xref:Microsoft.Office.Interop.Excel._Worksheet.Protect%2A> method of the active worksheet.

     ### [C#](#tab/csharp)
     :::code language="csharp" source="../vsto/codesnippet/CSharp/trin_vstcoreexcelautomationaddin/ThisAddIn.cs" id="Snippet17":::

     ### [VB](#tab/vb)
     :::code language="vb" source="../vsto/codesnippet/VisualBasic/trin_vstcoreexcelautomationaddin/ThisAddIn.vb" id="Snippet17":::
     ---

## Related content
- [Work with worksheets](../vsto/working-with-worksheets.md)
- [How to: Programmatically remove protection from worksheets](../vsto/how-to-programmatically-remove-protection-from-worksheets.md)
- [How to: Programmatically protect workbooks](../vsto/how-to-programmatically-protect-workbooks.md)
- [How to: Programmatically hide worksheets](../vsto/how-to-programmatically-hide-worksheets.md)
- [Host items and host controls overview](../vsto/host-items-and-host-controls-overview.md)
- [Worksheet host item](../vsto/worksheet-host-item.md)
- [Global access to objects in Office projects](../vsto/global-access-to-objects-in-office-projects.md)
- [Optional parameters in Office solutions](../vsto/optional-parameters-in-office-solutions.md)
