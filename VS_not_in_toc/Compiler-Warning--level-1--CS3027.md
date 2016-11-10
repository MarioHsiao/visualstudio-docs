---
title: "Compiler Warning (level 1) CS3027"
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
ms.assetid: c515e623-3f5a-49fa-a878-f1d8e90fdc24
caps.latest.revision: 3
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
# Compiler Warning (level 1) CS3027
'type_1' is not CLS-compliant because base interface 'type_2' is not CLS-compliant  
  
 A non-CLS compliant type cannot be a base type for a type that is CLS compliant.  
  
## Example  
 The following sample contains an interface with a method that uses a non-CLS compliant type in its signature, making the type non-CLS compliant.  
  
```  
// CS3027.cs  
// compile with: /target:library  
public interface IBase  
{  
   void IMethod(uint i);  
}  
```  
  
## Example  
 The following sample generates CS3027.  
  
```  
// CS3027_b.cs  
// compile with: /reference:CS3027.dll /target:library /W:1  
[assembly:System.CLSCompliant(true)]  
public interface IDerived : IBase {}  
```