---
description: "GetObjectOwner Method (ADOX)"
title: "GetObjectOwner Method (ADOX) | Microsoft Docs"
ms.prod: sql
ms.prod_service: connectivity
ms.technology: ado
ms.custom: ""
ms.date: "01/19/2017"
ms.reviewer: ""
ms.topic: reference
apitype: "COM"
f1_keywords: 
  - "_Catalog::raw_GetObjectOwner"
  - "_Catalog::GetObjectOwner"
helpviewer_keywords: 
  - "GetObjectOwner method [ADOX]"
ms.assetid: 8965adf0-9075-4125-8142-73eb700029c3
author: rothja
ms.author: jroth
---
# GetObjectOwner Method (ADOX)
Returns the owner of an object in a [Catalog](./catalog-object-adox.md).  
  
## Syntax  
  
```  
  
Owner = Catalog.GetObjectOwner(ObjectName, ObjectType [,ObjectTypeId])  
```  
  
## Return Value  
 Returns a **String** value that specifies the [Name](./name-property-adox.md) of the [User](./user-object-adox.md) or [Group](./group-object-adox.md) that owns the object.  
  
#### Parameters  
 *ObjectName*  
 A **String** value that specifies the name of the object for which to return the owner.  
  
 *ObjectType*  
 A **Long** value which can be one of the [ObjectTypeEnum](./objecttypeenum.md) constants, that specifies the type of the object for which to get the owner.  
  
 *ObjectTypeId*  
 Optional. A **Variant** value that specifies the GUID for a provider object type not defined by the OLE DB specification. This parameter is required if *ObjectType* is set to **adPermObjProviderSpecific**; otherwise, it is not used.  
  
## Remarks  
 An error will occur if the provider does not support returning object owners.  
  
## Applies To  
 [Catalog Object (ADOX)](./catalog-object-adox.md)  
  
## See Also  
 [GetObjectOwner and SetObjectOwner Methods Example (VB)](./getobjectowner-and-setobjectowner-methods-example-vb.md)   
 [SetObjectOwner Method](./setobjectowner-method.md)