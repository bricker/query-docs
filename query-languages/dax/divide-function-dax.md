---
title: "DIVIDE Function (DAX) | Microsoft Docs"
ms.prod: dax
ms.date: 5/22/2018
ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# DIVIDE Function (DAX)
Performs division and returns alternate result or BLANK() on division by 0.  
  
## Syntax  
  
```  
DIVIDE(<numerator>, <denominator> [,<alternateresult>])  
```  
  
#### Parameters  
  
|Term|Definition|  
|--------|--------------|  
|**numerator**|The dividend or number to divide.|  
|**denominator**|The divisor or number to divide by.|  
|**alternateresult**|(Optional) The value returned when division by zero results in an error. When not provided, the default value is BLANK().|  
  
## Return Value  
A decimal number.  
  
## Remarks  
Alternate result on divide by 0 must be a constant.  
  
## Example  
The following example returns 2.5.  
  
```  
=DIVIDE(5,2)  
```  
  
## Example  
The following example returns BLANK.  
  
```  
=DIVIDE(5,0)  
```  
  
## Example  
The following example returns 1.  
  
```  
=DIVIDE(5,0,1)  
```  
  
## See Also  
[QUOTIENT Function &#40;DAX&#41;](quotient-function-dax.md)  
[Math and Trig Functions &#40;DAX&#41;](math-and-trig-functions-dax.md)  
  