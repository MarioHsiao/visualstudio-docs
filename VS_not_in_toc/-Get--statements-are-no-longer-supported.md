---
title: "&#39;Get&#39; statements are no longer supported"
ms.custom: na
ms.date: 10/10/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 8d798357-7efb-4423-9808-8b20777b97ba
caps.latest.revision: 9
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
# &#39;Get&#39; statements are no longer supported
`Get` statements are no longer supported. File I/O functionality is available in the `Microsoft.VisualBasic` namespace.  
  
 `Get` is not supported for file operations, and can only be used in property procedure syntax.  
  
 **Error ID:** BC30829  
  
### To correct this error  
  
1.  Perform file operations using the members of `System.IO`, `FileSystemObject`, and Visual Basic run-time functions.  
  
## See Also  
 [Processing Drives, Directories, and Files](../Topic/Processing%20Drives,%20Directories,%20and%20Files%20\(Visual%20Basic\).md)   
 [Get Statement](../Topic/Get%20Statement.md)   
 [File Access with Visual Basic](../Topic/File%20Access%20with%20Visual%20Basic.md)