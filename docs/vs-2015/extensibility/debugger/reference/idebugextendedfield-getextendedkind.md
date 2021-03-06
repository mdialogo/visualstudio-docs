---
title: "IDebugExtendedField::GetExtendedKind | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-sdk"
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "IDebugExtendedField::GetExtendedKind"
  - "GetExtendedKind"
ms.assetid: 20dc1c13-3cc0-4bb4-9c99-fa85587c86c3
caps.latest.revision: 10
ms.author: "gregvanl"
manager: "ghogen"
---
# IDebugExtendedField::GetExtendedKind
[!INCLUDE[vs2017banner](../../../includes/vs2017banner.md)]

The latest version of this topic can be found at [IDebugExtendedField::GetExtendedKind](https://docs.microsoft.com/visualstudio/extensibility/debugger/reference/idebugextendedfield-getextendedkind).  
  
Retrieves the specified extended field kind.  
  
## Syntax  
  
```cpp#  
HRESULT GetExtendedKind(  
   FIELD_KIND_EX* pdwKind  
);  
```  
  
```csharp  
int GetExtendedKind(  
   ref enum_FIELD_KIND_EX pdwKind  
);  
```  
  
#### Parameters  
 `pdwKind`  
 [in, out] Value from the [FIELD_KIND_EX](../../../extensibility/debugger/reference/field-kind-ex.md) enumeration that defines the kind of field.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns an error code.  
  
## See Also  
 [IDebugExtendedField](../../../extensibility/debugger/reference/idebugextendedfield.md)

