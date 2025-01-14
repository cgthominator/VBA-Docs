---
title: SharedWorkspace.Links property (Office)
keywords: vbaof11.chm276006
f1_keywords:
- vbaof11.chm276006
ms.prod: office
api_name:
- Office.SharedWorkspace.Links
ms.assetid: 7389c657-8028-3914-cb03-5f2f50c448b5
ms.date: 01/24/2019
ms.localizationpriority: medium
---


# SharedWorkspace.Links property (Office)

Gets a **[SharedWorkspaceLinks](Office.SharedWorkspaceLinks.md)** collection that represents the list of links saved in the current shared workspace. Read-only.

> [!NOTE] 
> Beginning with Microsoft Office 2010, this object or member has been deprecated and should not be used.


## Syntax

_expression_.**Links**

_expression_ A variable that represents a **[SharedWorkspace](Office.SharedWorkspace.md)** object.


## Example

The following example lists the links saved in the current shared workspace.


```vb
  Dim swsLinks As Office.SharedWorkspaceLinks 
    Set swsLinks = ActiveWorkbook.SharedWorkspace.Links 
    MsgBox "There are " & swsLinks.Count & _ 
        " link(s) in the current shared workspace.", _ 
        vbInformation + vbOKOnly, _ 
        "Collection Information" 
    Set swsLinks = Nothing 

```


## See also

- [SharedWorkspace object members](overview/Library-Reference/sharedworkspace-members-office.md)



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]