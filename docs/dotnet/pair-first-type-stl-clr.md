---
title: "pair::first_type (STL/CLR) | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: ["cpp-windows"]
ms.tgt_pltfrm: ""
ms.topic: "reference"
f1_keywords: ["cliext::pair::first_type"]
dev_langs: ["C++"]
helpviewer_keywords: ["first_type member [STL/CLR]"]
ms.assetid: 8a7792ee-a2f6-4e17-9d0b-9c78007202d9
caps.latest.revision: 9
author: "mikeblome"
ms.author: "mblome"
manager: "ghogen"
ms.workload: ["cplusplus", "dotnet"]
---
# pair::first_type (STL/CLR)
The type of the first wrapped value.  
  
## Syntax  
  
```  
typedef Value1 first_type;  
```  
  
## Remarks  
 The type is a synonym for the template parameter `Value1`.  
  
## Example  
  
```  
// cliext_pair_first_type.cpp   
// compile with: /clr   
#include <cliext/utility>   
  
int main()   
    {   
    cliext::pair<wchar_t, int> c1(L'x', 3);   
    System::Console::WriteLine("[{0}, {1}]", c1.first, c1.second);   
  
    cliext::pair<wchar_t, int>::first_type first_val = c1.first;   
    cliext::pair<wchar_t, int>::second_type second_val = c1.second;   
    System::Console::WriteLine("[{0}, {1}]", first_val, second_val);   
    return (0);   
    }  
  
```  
  
```Output  
[x, 3]  
```  
  
## Requirements  
 **Header:** \<cliext/utility>  
  
 **Namespace:** cliext  
  
## See Also  
 [pair (STL/CLR)](../dotnet/pair-stl-clr.md)   
 [pair::first (STL/CLR)](../dotnet/pair-first-stl-clr.md)   
 [pair::second (STL/CLR)](../dotnet/pair-second-stl-clr.md)   
 [pair::second_type (STL/CLR)](../dotnet/pair-second-type-stl-clr.md)