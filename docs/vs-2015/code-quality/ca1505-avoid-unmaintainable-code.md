---
title: "CA1505: Avoid unmaintainable code | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology:
  - "vs-devops-test"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords:
  - "AvoidUnmaintainableCode"
  - "CA1505"
helpviewer_keywords:
  - "AvoidUnmaintainableCode"
  - "CA1505"
ms.assetid: 8292b268-5929-4221-b699-f9c414bcec5d
caps.latest.revision: 16
author: gewarren
ms.author: gewarren
manager: "wpickett"
---
# CA1505: Avoid unmaintainable code
[!INCLUDE[vs2017banner](../includes/vs2017banner.md)]

The latest version of this topic can be found at [CA1505: Avoid unmaintainable code](https://docs.microsoft.com/visualstudio/code-quality/ca1505-avoid-unmaintainable-code).

|||
|-|-|
|TypeName|AvoidUnmantainableCode|
|CheckId|CA1505|
|Category|Microsoft.Maintainability|
|Breaking Change|Non-breaking|

## Cause
 A type or method has a low maintainability index value.

## Rule Description
 The maintainability index is calculated by using the following metrics: lines of code, program volume, and cyclomatic complexity. Program volume is a measure of the difficulty of understanding of a type or method that is based on the number of operators and operands in the code. Cyclomatic complexity is a measure of the structural complexity of the type or method. You can learn more about code metrics at [Measuring Complexity and Maintainability of Managed Code](../code-quality/measuring-complexity-and-maintainability-of-managed-code.md).

 A low maintainability index indicates that a type or method is probably difficult to maintain and would be a good candidate to redesign.

## How to Fix Violations
 To fix this violation, redesign the type or method and try to split it into smaller and more focused types or methods.

## When to Suppress Warnings
 Exclude this warning when a type or method is still considered maintainable despite its large size or when the type or method cannot be split.

## See Also
 [Maintainability Warnings](../code-quality/maintainability-warnings.md)
 [Measuring Complexity and Maintainability of Managed Code](../code-quality/measuring-complexity-and-maintainability-of-managed-code.md)



