---
title: "&#39;Handles&#39; in modules must specify a &#39;WithEvents&#39; variable qualified with a single identifier"
ms.custom: na
ms.date: 10/01/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 7d866577-1e42-43f1-85d1-5d7eeba881b2
caps.latest.revision: 11
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
# &#39;Handles&#39; in modules must specify a &#39;WithEvents&#39; variable qualified with a single identifier
To specify an event handler, `Handles` statements must specify an object variable that was declared with the `WithEvents` keyword.  
  
 **Error ID:** BC31418  
  
### To correct this error  
  
-   Use the `WithEvents` modifier to declare variables that will be used with the `Handles` statement.  
  
## See Also  
 [Handles](../Topic/Handles%20Clause%20\(Visual%20Basic\).md)   
 [WithEvents](../Topic/WithEvents%20\(Visual%20Basic\).md)   
 [Events](../Topic/Events%20\(Visual%20Basic\).md)