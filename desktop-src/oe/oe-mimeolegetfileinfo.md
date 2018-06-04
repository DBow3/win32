---
title: MimeOleGetFileInfo function
description: Do not use. Returns file information for a supplied file path string.
ms.assetid: e3e6ad6e-101b-4adf-aa23-76e6352e42b5
keywords:
- MimeOleGetFileInfo function Windows Mail (formerly Outlook Express)
topic_type:
- apiref
api_name:
- MimeOleGetFileInfo
api_location:
- Inetcomm.dll
api_type:
- DllExport
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# MimeOleGetFileInfo function

Do not use. Returns file information for a supplied file path string.

## Syntax


```C++
HRESULT MimeOleGetFileInfo(
  _In_  LPSTR pszFilePath,
  _Out_ LPSTR *ppszCntType,
  _Out_ LPSTR *ppszSubType,
  _Out_ LPSTR *ppszCntDesc,
  _Out_ LPSTR *ppszFileName,
  _Out_ LPSTR *ppszExtension
);
```



## Parameters

<dl> <dt>

*pszFilePath* \[in\]
</dt> <dd>

Type: **LPSTR**

Specifies an **LPSTR** that contains the file path.

</dd> <dt>

*ppszCntType* \[out\]
</dt> <dd>

Type: **LPSTR\***

Receives a pointer to an **LPSTR** that contains the primary [Content-Type](http://msdn.microsoft.com/library/cdosys/html/48f7ae1c-9dc8-4b2f-8dc1-11c55e62173f.asp).

</dd> <dt>

*ppszSubType* \[out\]
</dt> <dd>

Type: **LPSTR\***

Receives a pointer to an **LPSTR** that contains the secondary [Content-Type](http://msdn.microsoft.com/library/cdosys/html/48f7ae1c-9dc8-4b2f-8dc1-11c55e62173f.asp).

</dd> <dt>

*ppszCntDesc* \[out\]
</dt> <dd>

Type: **LPSTR\***

Receives a pointer to an **LPSTR** that may contain the following descriptions: SHGFI\_USEFILEATTRIBUTES, SHGFI\_DISPLAYNAME, SHGFI\_TYPENAME. See shellapi.h.

</dd> <dt>

*ppszFileName* \[out\]
</dt> <dd>

Type: **LPSTR\***

Receives the file name.

</dd> <dt>

*ppszExtension* \[out\]
</dt> <dd>

Type: **LPSTR\***

Receives the file name extension.

</dd> </dl>

## Return value

Type: **HRESULT**

Returns one of the following values.



| Return code                                                                                   | Description                                                 |
|-----------------------------------------------------------------------------------------------|-------------------------------------------------------------|
| <dl> <dt>**S\_OK**</dt> </dl>          | Indicates success. <br/>                              |
| <dl> <dt>**E\_INVALIDARG**</dt> </dl>  | Indicates that a pointer parameter is **NULL**. <br/> |
| <dl> <dt>**E\_OUTOFMEMORY**</dt> </dl> | Indicates that an allocation failed. <br/>            |



 

## Remarks

Enter **NULL** for any parameter you do not wish to obtain info for. However, any parameter that is not **NULL** must be a valid pointer.

> [!Note]  
> Both *ppszCntType* and *ppszSubType* must be present and valid to receive info for either one.

 

## Requirements



|                                     |                                                                                                                |
|-------------------------------------|----------------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows XP \[desktop apps only\]<br/>                                                                    |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                                           |
| Product<br/>                  | Outlook Express 6.0<br/>                                                                                 |
| Header<br/>                   | <dl> <dt>Mimeole.h</dt> </dl>                           |
| Library<br/>                  | <dl> <dt>Inetcomm.lib</dt> </dl>                        |
| DLL<br/>                      | <dl> <dt>Inetcomm.dll (version 6.0 or later)</dt> </dl> |



## See also

<dl> <dt>

[**MimeOleGetFileInfoW**](oe-mimeolegetfileinfow.md)
</dt> </dl>

 

 




