---
title: KSMETHODSETID\_BdaDeviceConfiguration
description: KSMETHODSETID\_BdaDeviceConfiguration
ms.assetid: a0014869-2ea0-4f55-be3a-da1e624ad61c
ms.author: windowsdriverdev
ms.date: 11/28/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# KSMETHODSETID\_BdaDeviceConfiguration


## <span id="ddk_ksmethodsetid_bdadeviceconfiguration_ks"></span><span id="DDK_KSMETHODSETID_BDADEVICECONFIGURATION_KS"></span>


KSMETHODSETID\_BdaDeviceConfiguration is the BDA device configuration method set. It is used to configure a filter for a filter graph.

The following methods are available:

<span id="KSMETHOD_BDA_CREATE_PIN_FACTORY"></span><span id="ksmethod_bda_create_pin_factory"></span>[**KSMETHOD\_BDA\_CREATE\_PIN\_FACTORY**](ksmethod-bda-create-pin-factory.md)  
Triggers a call that creates a pin factory for the filter.

<span id="KSMETHOD_BDA_DELETE_PIN_FACTORY"></span><span id="ksmethod_bda_delete_pin_factory"></span>[**KSMETHOD\_BDA\_DELETE\_PIN\_FACTORY**](ksmethod-bda-delete-pin-factory.md)  
Triggers a call that deletes a pin factory for the filter.

<span id="KSMETHOD_BDA_CREATE_TOPOLOGY"></span><span id="ksmethod_bda_create_topology"></span>[**KSMETHOD\_BDA\_CREATE\_TOPOLOGY**](ksmethod-bda-create-topology.md)  
Creates a topology structure in Ring 3 that reflects the known connections in the filter.

### <span id="comments"></span><span id="COMMENTS"></span>Comments

This method set is implemented on filters.

If a BDA minidriver does not define it's own handlers for the methods in this method set, then the BDA support library will add default handlers when the BDA minidriver calls the **BdaInitFilter** function.

### <span id="see_also"></span><span id="SEE_ALSO"></span>See Also

[**BdaInitFilter**](https://msdn.microsoft.com/library/windows/hardware/ff556464)

 

 





