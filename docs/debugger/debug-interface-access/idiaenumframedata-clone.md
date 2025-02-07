---
description: "Creates an enumerator that contains the same enumeration state as the current frame data enumerator."
title: "IDiaEnumFrameData::Clone"
ms.date: "11/04/2016"
ms.topic: "reference"
dev_langs:
  - "C++"
helpviewer_keywords:
  - "IDiaEnumFrameData::Clone Method"
author: "mikejo5000"
ms.author: "mikejo"
manager: jmartens
ms.subservice: debug-diagnostics
---
# IDiaEnumFrameData::Clone

Creates an enumerator that contains the same enumeration state as the current enumerator.

## Syntax

```C++
HRESULT Clone( 
   IDiaEnumFrameData** ppenum
);
```

#### Parameters
 ppenum

[out] Returns an [IDiaEnumFrameData](../../debugger/debug-interface-access/idiaenumframedata.md) object that contains a duplicate  of the enumerator. The frame data is not duplicated, only the enumerator.

## Return Value
 If successful, returns `S_OK`; otherwise, returns an error code.

## See also
- [IDiaEnumFrameData](../../debugger/debug-interface-access/idiaenumframedata.md)
