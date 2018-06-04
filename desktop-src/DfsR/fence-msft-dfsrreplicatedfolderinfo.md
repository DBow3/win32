---
title: Fence method of the MSFT\_DfsrReplicatedFolderInfo class
description: Applies a fence to a specific file or directory.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: 20f3d749-2ad1-475c-9159-e279d47a6726
ms.prod: windows-server-dev
ms.technology:
- distributed-file-system-replication
- windows-management-instrumentation
ms.tgt_platform: multiple
keywords:
- Fence method Distributed File System Replication
- Fence method Distributed File System Replication , MSFT_DfsrReplicatedFolderInfo class
- MSFT_DfsrReplicatedFolderInfo class Distributed File System Replication , Fence method
topic_type:
- apiref
api_name:
- MSFT_DfsrReplicatedFolderInfo.Fence
api_location:
- DfsRWmiV2.dll
api_type:
- COM
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Fence method of the MSFT\_DfsrReplicatedFolderInfo class

Applies a fence to a specific file or directory.

## Syntax


```mof
uint32 Fence(
  [in] uint8   Mode,
  [in] string  FilePath,
  [in] boolean IsRecursive
);
```



## Parameters

<dl> <dt>

*Mode* \[in\]
</dt> <dd>

Fencing mode. This parameter can be one of the following values.

<dt>

<span id="Unfence"></span><span id="unfence"></span><span id="UNFENCE"></span>

<span id="Unfence"></span><span id="unfence"></span><span id="UNFENCE"></span>**Unfence** (0)


</dt> <dd>

This file or folder will lose all conflicts.

</dd> <dt>

<span id="Initial_Sync"></span><span id="initial_sync"></span><span id="INITIAL_SYNC"></span>

<span id="Initial_Sync"></span><span id="initial_sync"></span><span id="INITIAL_SYNC"></span>**Initial Sync** (1)


</dt> <dd>

Initial fence value for non-primary member.

</dd> <dt>

<span id="Initial_Primary"></span><span id="initial_primary"></span><span id="INITIAL_PRIMARY"></span>

<span id="Initial_Primary"></span><span id="initial_primary"></span><span id="INITIAL_PRIMARY"></span>**Initial Primary** (2)


</dt> <dd>

Initial fence value for primary member.

</dd> <dt>

<span id="Default"></span><span id="default"></span><span id="DEFAULT"></span>

<span id="Default"></span><span id="default"></span><span id="DEFAULT"></span>**Default** (3)


</dt> <dd>

Default fencing value.

</dd> <dt>

<span id="Fence"></span><span id="fence"></span><span id="FENCE"></span>

<span id="Fence"></span><span id="fence"></span><span id="FENCE"></span>**Fence** (4)


</dt> <dd>

Fence with current time stamp.

</dd> </dl> </dd> <dt>

*FilePath* \[in\]
</dt> <dd>

The full path to the fence.

</dd> <dt>

*IsRecursive* \[in\]
</dt> <dd>

Indicates whether to apply the fence recursively to all children.

</dd> </dl>

## Return value

This method returns one of the [MONITOR\_STATUS return codes](monitor-status-return-codes.md) or one of the [system error codes](https://msdn.microsoft.com/library/windows/desktop/ms681381).

## Requirements



|                                     |                                                                                          |
|-------------------------------------|------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                                |
| Minimum supported server<br/> | Windows Server 2012 R2<br/>                                                        |
| Namespace<br/>                | Root\\Microsoft\\Windows\\Dfsr<br/>                                                |
| MOF<br/>                      | <dl> <dt>Dfsrwmiv2.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>DfsRWmiV2.dll</dt> </dl> |



## See also

<dl> <dt>

[**MSFT\_DfsrReplicatedFolderInfo**](msft-dfsrreplicatedfolderinfo.md)
</dt> </dl>

 

 




