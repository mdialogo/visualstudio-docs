---
title: "IDebugCoreServer3::DiagnoseWebDebuggingError | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-sdk"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "IDebugCoreServer3::DiagnoseWebDebuggingError"
helpviewer_keywords: 
  - "IDebugCoreServer3::DiagnoseWebDebuggingError"
ms.assetid: 8c4570ca-ae55-42f2-bbaa-8d8e75d2fa19
caps.latest.revision: 9
ms.author: "gregvanl"
manager: "ghogen"
---
# IDebugCoreServer3::DiagnoseWebDebuggingError
[!INCLUDE[vs2017banner](../../../includes/vs2017banner.md)]

The latest version of this topic can be found at [IDebugCoreServer3::DiagnoseWebDebuggingError](https://docs.microsoft.com/visualstudio/extensibility/debugger/reference/idebugcoreserver3-diagnosewebdebuggingerror).  
  
Attempts to determine why an auto-attach failed.  
  
## Syntax  
  
```cpp#  
HRESULT DiagnoseWebDebuggingError(  
   LPCWSTR pszUrl  
);  
```  
  
```csharp  
int DiagnoseWebDebuggingError(  
   string pszUrl  
);  
```  
  
#### Parameters  
 `pszUrl`  
 [in] Not currently used; should always be set to a null value.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns an error code. The following are other typical return codes:  
  
|Code|Description|  
|----------|-----------------|  
|`S_WEBDBG_UNABLE_TO_DIAGNOSE`|Cannot determine why the remote server failed to start debugging.|  
|`S_WEBDBG_DEBUG_VERB_BLOCKED`|Cannot debug on remote server, possibly due to insufficient permissions or because the DEBUG verb is not enabled.|  
|`E_WEBDBG_DEBUG_VERB_BLOCKED`|The web server has been locked down and is blocking the DEBUG verb, which is required to enable debugging.|  
  
## See Also  
 [IDebugCoreServer3](../../../extensibility/debugger/reference/idebugcoreserver3.md)

