---
title: Policy CSP - Storage
description: Policy CSP - Storage
ms.author: maricia
ms.topic: article
ms.prod: w10
ms.technology: windows
author: MariciaAlforque
ms.date: 03/12/2018
---

# Policy CSP - Storage



<hr/>

<!--Policies-->
## Storage policies  

<dl>
  <dd>
    <a href="#storage-allowdiskhealthmodelupdates">Storage/AllowDiskHealthModelUpdates</a>
  </dd>
  <dd>
    <a href="#storage-enhancedstoragedevices">Storage/EnhancedStorageDevices</a>
  </dd>
</dl>


<hr/>

<!--Policy-->
<a href="" id="storage-allowdiskhealthmodelupdates"></a>**Storage/AllowDiskHealthModelUpdates**  

<!--SupportedSKUs-->
<table>
<tr>
	<th>Home</th>
	<th>Pro</th>
	<th>Business</th>
	<th>Enterprise</th>
	<th>Education</th>
	<th>Mobile</th>
	<th>Mobile Enterprise</th>
</tr>
<tr>
	<td><img src="images/crossmark.png" alt="cross mark" /></td>
	<td><img src="images/checkmark.png" alt="check mark" /><sup>3</sup></td>
	<td><img src="images/checkmark.png" alt="check mark" /><sup>3</sup></td>
	<td><img src="images/checkmark.png" alt="check mark" /><sup>3</sup></td>
	<td><img src="images/checkmark.png" alt="check mark" /><sup>3</sup></td>
	<td><img src="images/crossmark.png" alt="cross mark" /></td>
	<td><img src="images/crossmark.png" alt="cross mark" /></td>
</tr>
</table>

<!--/SupportedSKUs-->
<!--Scope-->
[Scope](./policy-configuration-service-provider.md#policy-scope):

> [!div class = "checklist"]
> * Device

<hr/>

<!--/Scope-->
<!--Description-->
Added in Windows 10, version 1709.  Allows disk health model updates.



Value type is integer.

<!--/Description-->
<!--ADMXMapped-->
ADMX Info:  
-   GP English name: *Allow downloading updates to the Disk Failure Prediction Model*
-   GP name: *SH_AllowDiskHealthModelUpdates*
-   GP path: *System/Storage Health*
-   GP ADMX file name: *StorageHealth.admx*

<!--/ADMXMapped-->
<!--SupportedValues-->
The following list shows the supported values:

-   0 - Do not allow
-   1 (default) - Allow

<!--/SupportedValues-->
<!--/Policy-->

<hr/>

<!--Policy-->
<a href="" id="storage-enhancedstoragedevices"></a>**Storage/EnhancedStorageDevices**  

<!--SupportedSKUs-->
<table>
<tr>
	<th>Home</th>
	<th>Pro</th>
	<th>Business</th>
	<th>Enterprise</th>
	<th>Education</th>
	<th>Mobile</th>
	<th>Mobile Enterprise</th>
</tr>
<tr>
	<td><img src="images/crossmark.png" alt="cross mark" /></td>
	<td><img src="images/checkmark.png" alt="check mark" /></td>
	<td><img src="images/checkmark.png" alt="check mark" /></td>
	<td><img src="images/checkmark.png" alt="check mark" /></td>
	<td><img src="images/checkmark.png" alt="check mark" /></td>
	<td><img src="images/crossmark.png" alt="cross mark" /></td>
	<td><img src="images/crossmark.png" alt="cross mark" /></td>
</tr>
</table>

<!--/SupportedSKUs-->
<!--Scope-->
[Scope](./policy-configuration-service-provider.md#policy-scope):

> [!div class = "checklist"]
> * Device

<hr/>

<!--/Scope-->
<!--Description-->
This policy setting configures whether or not Windows will activate an Enhanced Storage device.

If you enable this policy setting, Windows will not activate unactivated Enhanced Storage devices.

If you disable or do not configure this policy setting, Windows will activate unactivated Enhanced Storage devices.

<!--/Description-->
> [!TIP]
> This is an ADMX-backed policy and requires a special SyncML format to enable or disable.  For details, see [Understanding ADMX-backed policies](./understanding-admx-backed-policies.md).

> You must specify the data type in the SyncML as &lt;Format&gt;chr&lt;/Format&gt;. For an example SyncML, refer to [Enabling a policy](./understanding-admx-backed-policies.md#enabling-a-policy).

> The payload of the SyncML must be XML-encoded; for this XML encoding, there are a variety of online encoders that you can use. To avoid encoding the payload, you can use CDATA if your MDM supports it.  For more information, see [CDATA Sections](http://www.w3.org/TR/REC-xml/#sec-cdata-sect).

<!--ADMXBacked-->
ADMX Info:  
-   GP English name: *Do not allow Windows to activate Enhanced Storage devices*
-   GP name: *TCGSecurityActivationDisabled*
-   GP path: *System/Enhanced Storage Access*
-   GP ADMX file name: *enhancedstorage.admx*

<!--/ADMXBacked-->
<!--/Policy-->
<hr/>

Footnote:

-   1 - Added in Windows 10, version 1607.
-   2 - Added in Windows 10, version 1703.
-   3 - Added in Windows 10, version 1709.
-   4 - Added in Windows 10, version 1803.

<!--/Policies-->

