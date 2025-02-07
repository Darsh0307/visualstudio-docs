---
title: "FormatUrl Task"
description: Learn about how to use the MSBuild FormatUrl task to convert an input URL to a correct output URL format.
ms.date: "11/04/2016"
ms.topic: "reference"
dev_langs:
  - "VB"
  - "CSharp"
  - "C++"
helpviewer_keywords:
  - "MSBuild, FormatUrl task"
  - "FormatUrl task [MSBuild]"
author: ghogen
ms.author: ghogen
manager: jmartens
ms.subservice: msbuild
---
# FormatUrl task

Converts a URL to a correct URL format.

## Parameters

 The following table describes the parameters of the `FormatUrl` task.

|Parameter|Description|
|---------------|-----------------|
|`InputUrl`|Optional `String` parameter.<br /><br /> Specifies the URL to format.|
|`OutputUrl`|Optional `String` output parameter.<br /><br /> Specifies the formatted URL.|

## Remarks

 In addition to having the parameters that are listed in the table, this task inherits parameters from the <xref:Microsoft.Build.Tasks.TaskExtension> class, which itself inherits from the <xref:Microsoft.Build.Utilities.Task> class. For a list of these additional parameters and their descriptions, see [TaskExtension base class](../msbuild/taskextension-base-class.md).

## See also

- [Tasks](../msbuild/msbuild-tasks.md)
- [Task reference](../msbuild/msbuild-task-reference.md)