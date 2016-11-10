---
title: "XML elements cannot be selected from type &#39;type&#39;"
ms.custom: na
ms.date: 10/01/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 01c19899-2b44-41e9-a99c-35edfa0deaf1
caps.latest.revision: 5
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
# XML elements cannot be selected from type &#39;type&#39;
An XML child element has been referenced for an object that is not of type <xref:System.Xml.Linq.XElement?qualifyHint=False>, <xref:System.Xml.Linq.XDocument?qualifyHint=False>, or `IEnumerable(Of XElement)`. For more information, see [XML Child Axis Property](../Topic/XML%20Child%20Axis%20Property%20\(Visual%20Basic\).md).  
  
```vb#  
' Generates an error.  
Dim var = "sample text".<child>  
```  
  
 **Error ID:** BC36807  
  
### To correct this error  
  
-   Ensure that the object of which you are referencing an attribute is strongly typed as <xref:System.Xml.Linq.XElement?qualifyHint=False>, <xref:System.Xml.Linq.XDocument?qualifyHint=False>, or `IEnumerable(Of XElement)`. Following is an example:  
  
    ```vb#  
    Dim elem As XElement = <root>  
                             <child />  
                           </root>  
    Dim var = elem.<child>  
    ```  
  
## See Also  
 [XML Child Axis Property](../Topic/XML%20Child%20Axis%20Property%20\(Visual%20Basic\).md)   
 [XML Axis Properties](../Topic/XML%20Axis%20Properties%20\(Visual%20Basic\).md)   
 [XML](../Topic/XML%20in%20Visual%20Basic.md)