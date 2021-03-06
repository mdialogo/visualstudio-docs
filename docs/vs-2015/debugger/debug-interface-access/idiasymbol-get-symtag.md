---
title: "IDiaSymbol::get_symTag | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-debug"
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "IDiaSymbol::get_symTag method"
ms.assetid: 139a35bd-faeb-4878-be72-394dedfbb18f
caps.latest.revision: 11
author: "mikejo5000"
ms.author: "mikejo"
manager: "ghogen"
---
# IDiaSymbol::get_symTag
[!INCLUDE[vs2017banner](../../includes/vs2017banner.md)]

The latest version of this topic can be found at [IDiaSymbol::get_symTag](https://docs.microsoft.com/visualstudio/debugger/debug-interface-access/idiasymbol-get-symtag).  
  
Retrieves the symbol type classifier.  
  
## Syntax  
  
```cpp#  
HRESULT get_symTag (   
   DWORD* pRetVal  
);  
```  
  
#### Parameters  
 `pRetVal`  
 [out] Returns A value from the [SymTagEnum Enumeration](../../debugger/debug-interface-access/symtagenum.md) enumeration that specifies the symbol type classifier.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns `S_FALSE` or an error code.  
  
> [!NOTE]
>  A return value of `S_FALSE` means the property is not available for the symbol.  
  
## Example  
  
```cpp#  
IDiaSymbol* pType;  
DWORD       tag = 0;  
pType->get_symTag( &tag );  
```  
  
## See Also  
 [IDiaSymbol](../../debugger/debug-interface-access/idiasymbol.md)   
 [SymTagEnum Enumeration](../../debugger/debug-interface-access/symtagenum.md)



