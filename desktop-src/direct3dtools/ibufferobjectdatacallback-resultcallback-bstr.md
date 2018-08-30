---
Description: A callback that notifies the host of buffer information written to a file by the assocaited request.
MS-HAID: vspixengine.IBufferObjectDataCallback\_ResultCallback\_BSTR
MSHAttr:
- PreferredSiteName:MSDN
- PreferredLib:/library/windows/desktop
title: IBufferObjectDataCallback::ResultCallback method
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# <span id="vspixengine.ibufferobjectdatacallback_resultcallback_bstr"></span>IBufferObjectDataCallback::ResultCallback method

A callback that notifies the host of buffer information written to a file by the assocaited request.

## Syntax


```C++
);
```

## Parameters

*File*   
A COM string that contains the pathname of the file where results are written.

## Return value

If this method succeeds, it returns **S\_OK**. Otherwise, it returns an **HRESULT** error code.

## Requirements

<table><colgroup><col style="width: 50%" /><col style="width: 50%" /></colgroup><tbody><tr class="odd"><td><p>Header</p></td><td>Vspixengine.h</td></tr></tbody></table>

## <span id="see_also"></span>See also

[**IBufferObjectDataCallback**](https://msdn.microsoft.com/library/windows/desktop/mt422646)

 

 


