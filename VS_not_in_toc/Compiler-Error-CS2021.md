---
title: "Compiler Error CS2021"
ms.custom: na
ms.date: 10/01/2016
ms.devlang: 
  - CSharp
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 8379d77e-6586-4e43-9aab-7cdf3ffecf51
caps.latest.revision: 6
manager: douge
translation.priority.ht: 
  - de-de
  - es-es
  - fr-fr
  - it-it
  - ja-jp
  - ko-kr
  - ru-ru
  - zh-cn
  - zh-tw
translation.priority.mt: 
  - cs-cz
  - pl-pl
  - pt-br
  - tr-tr
---
# Compiler Error CS2021
File name 'file' is too long or invalid  
  
 All file names passed to the C# compiler must be no longer than `_MAX_PATH` (defined in a Windows header file). the compiler will give this error in the following situations:  
  
-   A file name (including the path) is longer than `_MAX_PATH`.  
  
-   The file name contains invalid characters.  
  
-   The file name contains wildcards where wildcards are not allowed (such as in resource file names).