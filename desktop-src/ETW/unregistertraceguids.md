---
Description: The UnregisterTraceGuids function unregisters an event trace provider and its event trace classes.
ms.assetid: 1fa10f66-a78b-4f40-9518-72d48365246e
title: UnregisterTraceGuids function
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# UnregisterTraceGuids function

The **UnregisterTraceGuids** function unregisters an event trace provider and its event trace classes.

## Syntax


```C++
ULONG UnregisterTraceGuids(
  _In_ TRACEHANDLE RegistrationHandle
);
```



## Parameters

<dl> <dt>

*RegistrationHandle* \[in\]
</dt> <dd>

Handle to the event trace provider, obtained from an earlier call to the [**RegisterTraceGuids**](registertraceguids.md) function.

</dd> </dl>

## Return value

If the function succeeds, the return value is ERROR\_SUCCESS.

If the function fails, the return value is one of the [system error codes](https://msdn.microsoft.com/windows/desktop/4a3a8feb-a05f-4614-8f04-1f507da7e5b7). The following table includes some common errors and their causes.



| Return code                                                                                              | Description                                                                                                         |
|----------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------|
| <dl> <dt>**ERROR\_INVALID\_PARAMETER**</dt> </dl> | The *RegistrationHandle* parameter does not specify the handle to a registered provider or is **NULL**. <br/> |



 

## Remarks

Providers call this function.

The event trace provider must have been registered previously by calling the [**RegisterTraceGuids**](registertraceguids.md) function.

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 2000 Professional \[desktop apps \| UWP apps\]<br/>                       |
| Minimum supported server<br/> | Windows 2000 Server \[desktop apps \| UWP apps\]<br/>                             |
| Minimum supported phone<br/>  | Windows Phone 8.1<br/>                                                            |
| Header<br/>                   | <dl> <dt>Evntrace.h</dt> </dl>   |
| Library<br/>                  | <dl> <dt>Advapi32.lib</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Advapi32.dll</dt> </dl> |



## See also

<dl> <dt>

[**RegisterTraceGuids**](registertraceguids.md)
</dt> </dl>

 

 



