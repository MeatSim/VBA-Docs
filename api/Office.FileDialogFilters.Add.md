---
title: FileDialogFilters.Add method (Office)
keywords: vbaof11.chm255006
f1_keywords:
- vbaof11.chm255006
ms.prod: office
api_name:
- Office.FileDialogFilters.Add
ms.assetid: f1ff515f-9049-189d-a67a-30198d55253b
ms.date: 01/09/2019
ms.localizationpriority: medium
---


# FileDialogFilters.Add method (Office)

Adds a new file filter to the list of filters in the **Files of type** drop-down list in the **File** dialog box. Returns a **FileDialogFilter** object that represents the newly added file filter.


## Syntax

_expression_.**Add** (_Description_, _Extensions_, _Position_)

_expression_ Required. A variable that represents a **[FileDialogFilters](Office.FileDialogFilters.md)** object.


## Parameters

|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _Description_|Required|**String**|The text representing the description of the file name extension that you want to add to the list of filters.|
| _Extensions_|Required|**String**|The text representing the file name extension you want to add to the list of filters. More than one extension may be specified, and each must be separated by a semi-colon. For example, the argument can be assigned to the string: "*.txt; *.htm".<br/><br/> **NOTE**: Parentheses don't need to be added around the extensions. Microsoft Office will automatically add parentheses around the extensions string when the description and extensions strings are concatenated into one file filter item.|
| _Position_|Optional|**Variant**|A number that indicates the position of the new control in the filter list. The new filter will be inserted before the filter at this position. If this argument is omitted, the filter is added at the end of the list.|

## Remarks

Each filter in a list is made up of two parts: the file name extension (that is, .txt) and the text description of the file name extension (that is, Text Files). Together, the file filter would appear in the **Files of type** list as: Text Files (*.txt). 

Note that when a filter is added to the list, the default filters are not removed. Filters are only displayed when the **Windows** option is checked. If _Position_ is invalid, an out-of-range run-time error is displayed. If the _Description_ and _Extensions_ values are invalid, a run-time error (parse) is displayed.


## See also

- [FileDialogFilters object members](overview/library-reference/filedialogfilters-members-office.md)

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]