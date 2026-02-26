# PropertyGroup(bpy_struct)

## Custom Properties

PropertyGroups are the base class for dynamically defined sets of properties.

They can be used to extend existing Blender data with your own types which can be animated, accessed from the user interface and from Python.

Note

The values assigned to Blender data are saved to disk but the class definitions are not, this means whenever you load Blender the class needs to be registered too.

This is best done by creating an add-on which loads on startup and registers your properties.

Note

PropertyGroups must be registered before assigning them to Blender data.

See also

Property types used in class declarations are all in [`bpy.props`](bpy.props.md#module-bpy.props "bpy.props")
    
    
    import bpy
    
    
    class MyPropertyGroup(bpy.types.PropertyGroup):
        custom_1: bpy.props.FloatProperty(name="My Float")
        custom_2: bpy.props.IntProperty(name="My Int")
    
    
    bpy.utils.register_class(MyPropertyGroup)
    
    bpy.types.Object.my_prop_grp = bpy.props.PointerProperty(type=MyPropertyGroup)
    
    
    # Test this worked.
    bpy.data.objects[0].my_prop_grp.custom_1 = 22.0
    

base class — [`bpy_struct`](bpy.types.bpy_struct.md#bpy.types.bpy_struct "bpy.types.bpy_struct")

subclasses — [`AssetHandle`](bpy.types.AssetHandle.md#bpy.types.AssetHandle "bpy.types.AssetHandle"), [`OperatorFileListElement`](bpy.types.OperatorFileListElement.md#bpy.types.OperatorFileListElement "bpy.types.OperatorFileListElement"), [`OperatorMousePath`](bpy.types.OperatorMousePath.md#bpy.types.OperatorMousePath "bpy.types.OperatorMousePath"), [`OperatorStrokeElement`](bpy.types.OperatorStrokeElement.md#bpy.types.OperatorStrokeElement "bpy.types.OperatorStrokeElement"), [`SelectedUvElement`](bpy.types.SelectedUvElement.md#bpy.types.SelectedUvElement "bpy.types.SelectedUvElement")

_class _bpy.types.PropertyGroup(_bpy_struct_)
    

Group of ID properties

name
    

Unique name used in the code and scripting

Type:
    

string, default “”, (never None)

_classmethod _bl_rna_get_subclass(_id_ , _default =None_, _/_)
    

Parameters:
    

**id** (_str_) – The RNA type identifier.

Returns:
    

The RNA type or default when not found.

Return type:
    

[`bpy.types.Struct`](bpy.types.Struct.md#bpy.types.Struct "bpy.types.Struct") subclass

_classmethod _bl_rna_get_subclass_py(_id_ , _default =None_, _/_)
    

Parameters:
    

**id** (_str_) – The RNA type identifier.

Returns:
    

The class or default when not found.

Return type:
    

type

### Inherited Properties

  * [`bpy_struct.id_data`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.id_data "bpy.types.bpy_struct.id_data")

| 


  
---|---  
  
### Inherited Functions

  * [`bpy_struct.as_pointer`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.as_pointer "bpy.types.bpy_struct.as_pointer")
  * [`bpy_struct.driver_add`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.driver_add "bpy.types.bpy_struct.driver_add")
  * [`bpy_struct.driver_remove`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.driver_remove "bpy.types.bpy_struct.driver_remove")
  * [`bpy_struct.get`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.get "bpy.types.bpy_struct.get")
  * [`bpy_struct.id_properties_clear`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.id_properties_clear "bpy.types.bpy_struct.id_properties_clear")
  * [`bpy_struct.id_properties_ensure`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.id_properties_ensure "bpy.types.bpy_struct.id_properties_ensure")
  * [`bpy_struct.id_properties_ui`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.id_properties_ui "bpy.types.bpy_struct.id_properties_ui")
  * [`bpy_struct.is_property_hidden`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.is_property_hidden "bpy.types.bpy_struct.is_property_hidden")
  * [`bpy_struct.is_property_overridable_library`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.is_property_overridable_library "bpy.types.bpy_struct.is_property_overridable_library")
  * [`bpy_struct.is_property_readonly`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.is_property_readonly "bpy.types.bpy_struct.is_property_readonly")
  * [`bpy_struct.is_property_set`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.is_property_set "bpy.types.bpy_struct.is_property_set")
  * [`bpy_struct.items`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.items "bpy.types.bpy_struct.items")

| 

  * [`bpy_struct.keyframe_delete`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.keyframe_delete "bpy.types.bpy_struct.keyframe_delete")
  * [`bpy_struct.keyframe_insert`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.keyframe_insert "bpy.types.bpy_struct.keyframe_insert")
  * [`bpy_struct.keys`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.keys "bpy.types.bpy_struct.keys")
  * [`bpy_struct.path_from_id`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.path_from_id "bpy.types.bpy_struct.path_from_id")
  * [`bpy_struct.path_resolve`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.path_resolve "bpy.types.bpy_struct.path_resolve")
  * [`bpy_struct.pop`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.pop "bpy.types.bpy_struct.pop")
  * [`bpy_struct.property_overridable_library_set`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.property_overridable_library_set "bpy.types.bpy_struct.property_overridable_library_set")
  * [`bpy_struct.property_unset`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.property_unset "bpy.types.bpy_struct.property_unset")
  * [`bpy_struct.rna_ancestors`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.rna_ancestors "bpy.types.bpy_struct.rna_ancestors")
  * [`bpy_struct.type_recast`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.type_recast "bpy.types.bpy_struct.type_recast")
  * [`bpy_struct.values`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.values "bpy.types.bpy_struct.values")

  
---|---  
  
### References

  * [`CollectionExport.export_properties`](bpy.types.CollectionExport.md#bpy.types.CollectionExport.export_properties "bpy.types.CollectionExport.export_properties")
  * [`PropertyGroupItem.collection`](bpy.types.PropertyGroupItem.md#bpy.types.PropertyGroupItem.collection "bpy.types.PropertyGroupItem.collection")

| 

  * [`PropertyGroupItem.group`](bpy.types.PropertyGroupItem.md#bpy.types.PropertyGroupItem.group "bpy.types.PropertyGroupItem.group")
  * [`PropertyGroupItem.idp_array`](bpy.types.PropertyGroupItem.md#bpy.types.PropertyGroupItem.idp_array "bpy.types.PropertyGroupItem.idp_array")

  
---|---
