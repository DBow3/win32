---
Description: Request for a tiled texture to be written as a DDS file.
MS-HAID: vspixengine.ITileRequest
MSHAttr:
- PreferredSiteName:MSDN
- PreferredLib:/library/windows/desktop
title: ITileRequest interface
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: interface
ms.date: 05/31/2018
---

# <span id="vspixengine.itilerequest"></span>ITileRequest interface

Request for a tiled texture to be written as a DDS file.

## Members

The **ITileRequest** interface inherits from the [**IUnknown**](https://msdn.microsoft.com/library/windows/desktop/ms680509) interface. **ITileRequest** also has these types of members:

-   [Methods](#methods)

### <span id="methods"></span>Methods

The **ITileRequest** interface has these methods.

<table><colgroup><col style="width: 50%" /><col style="width: 50%" /></colgroup><thead><tr class="header"><th style="text-align: left;">Method</th><th style="text-align: left;">Description</th></tr></thead><tbody><tr class="odd"><td style="text-align: left;"><a href="https://msdn.microsoft.com/library/windows/desktop/mt432820"><strong>RequestBufferTileAsync</strong></a></td><td style="text-align: left;"><p>Requests to get the raw contents of a tile.</p></td></tr><tr class="even"><td style="text-align: left;"><a href="https://msdn.microsoft.com/library/windows/desktop/mt432821"><strong>RequestTextureTileAsync</strong></a></td><td style="text-align: left;"><p>Requests to get the contents of a tiled texture as a .DDS (DirectDraw Surface) file.</p></td></tr></tbody></table>

 

## Requirements

<table><colgroup><col style="width: 50%" /><col style="width: 50%" /></colgroup><tbody><tr class="odd"><td><p>Header</p></td><td>Vspixengine.h</td></tr></tbody></table>

 

 


