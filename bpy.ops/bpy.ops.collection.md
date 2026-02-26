# Collection Operators

bpy.ops.collection.create(_*_ , _name ='Collection'_)
    

Create an object collection from selected objects

Parameters:
    

**name** (_string_ _,__(__optional_ _,__never None_ _)_) – Name, Name of the new collection

bpy.ops.collection.export_all()
    

Invoke all configured exporters on this collection

bpy.ops.collection.exporter_add(_*_ , _name =''_)
    

Add Exporter

Parameters:
    

**name** (_string_ _,__(__optional_ _,__never None_ _)_) – Name, FileHandler idname

bpy.ops.collection.exporter_export(_*_ , _index =0_)
    

Invoke the export operation

Parameters:
    

**index** (_int in_ _[__0_ _,__inf_ _]__,__(__optional_ _)_) – Index, Exporter index

bpy.ops.collection.exporter_remove(_*_ , _index =0_)
    

Remove Exporter

Parameters:
    

**index** (_int in_ _[__0_ _,__inf_ _]__,__(__optional_ _)_) – Index, Exporter index

bpy.ops.collection.objects_add_active(_*_ , _collection =''_)
    

Add selected objects to one of the collections the active-object is part of. Optionally add to “All Collections” to ensure selected objects are included in the same collections as the active object

Parameters:
    

**collection** (_enum in_ _[__]__,__(__optional_ _)_) – Collection, The collection to add other selected objects to

bpy.ops.collection.objects_remove(_*_ , _collection =''_)
    

Remove selected objects from a collection

Parameters:
    

**collection** (_enum in_ _[__]__,__(__optional_ _)_) – Collection, The collection to remove this object from

bpy.ops.collection.objects_remove_active(_*_ , _collection =''_)
    

Remove the object from an object collection that contains the active object

Parameters:
    

**collection** (_enum in_ _[__]__,__(__optional_ _)_) – Collection, The collection to remove other selected objects from

bpy.ops.collection.objects_remove_all()
    

Remove selected objects from all collections
