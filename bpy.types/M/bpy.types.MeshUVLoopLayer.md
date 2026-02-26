# MeshUVLoopLayer(bpy_struct)

base class — [`bpy_struct`](bpy.types.bpy_struct.html#bpy.types.bpy_struct "bpy.types.bpy_struct")

_class _bpy.types.MeshUVLoopLayer(_bpy_struct_)
    

active
    

Set the map as active for display and editing

Type:
    

boolean, default False

active_clone
    

Set the map as active for cloning

Type:
    

boolean, default False

active_render
    

Set the UV map as active for rendering

Type:
    

boolean, default False

data
    

Deprecated, use ‘uv’, ‘vertex_select’, ‘edge_select’ or ‘pin’ properties instead

Type:
    

[`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`MeshUVLoop`](bpy.types.MeshUVLoop.html#bpy.types.MeshUVLoop "bpy.types.MeshUVLoop"), (readonly)

edge_selection
    

Selection state of the edge in the UV editor

Type:
    

[`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`BoolAttributeValue`](bpy.types.BoolAttributeValue.html#bpy.types.BoolAttributeValue "bpy.types.BoolAttributeValue"), (readonly)

name
    

Name of UV map

Type:
    

string, default “”, (never None)

pin
    

UV pinned state in the UV editor

Type:
    

[`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`BoolAttributeValue`](bpy.types.BoolAttributeValue.html#bpy.types.BoolAttributeValue "bpy.types.BoolAttributeValue"), (readonly)

uv
    

UV coordinates on face corners

Type:
    

[`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`Float2AttributeValue`](bpy.types.Float2AttributeValue.html#bpy.types.Float2AttributeValue "bpy.types.Float2AttributeValue"), (readonly)

vertex_selection
    

Selection state of the face corner the UV editor

Type:
    

[`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`BoolAttributeValue`](bpy.types.BoolAttributeValue.html#bpy.types.BoolAttributeValue "bpy.types.BoolAttributeValue"), (readonly)

_classmethod _bl_rna_get_subclass(_id_ , _default =None_, _/_)
    

Parameters:
    

**id** (_str_) – The RNA type identifier.

Returns:
    

The RNA type or default when not found.

Return type:
    

[`bpy.types.Struct`](bpy.types.Struct.html#bpy.types.Struct "bpy.types.Struct") subclass

_classmethod _bl_rna_get_subclass_py(_id_ , _default =None_, _/_)
    

Parameters:
    

**id** (_str_) – The RNA type identifier.

Returns:
    

The class or default when not found.

Return type:
    

type

## Inherited Properties

  * [`bpy_struct.id_data`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.id_data "bpy.types.bpy_struct.id_data")

| 


  
---|---  
  
## Inherited Functions

  * [`bpy_struct.as_pointer`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.as_pointer "bpy.types.bpy_struct.as_pointer")
  * [`bpy_struct.driver_add`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.driver_add "bpy.types.bpy_struct.driver_add")
  * [`bpy_struct.driver_remove`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.driver_remove "bpy.types.bpy_struct.driver_remove")
  * [`bpy_struct.get`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.get "bpy.types.bpy_struct.get")
  * [`bpy_struct.id_properties_clear`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.id_properties_clear "bpy.types.bpy_struct.id_properties_clear")
  * [`bpy_struct.id_properties_ensure`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.id_properties_ensure "bpy.types.bpy_struct.id_properties_ensure")
  * [`bpy_struct.id_properties_ui`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.id_properties_ui "bpy.types.bpy_struct.id_properties_ui")
  * [`bpy_struct.is_property_hidden`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.is_property_hidden "bpy.types.bpy_struct.is_property_hidden")
  * [`bpy_struct.is_property_overridable_library`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.is_property_overridable_library "bpy.types.bpy_struct.is_property_overridable_library")
  * [`bpy_struct.is_property_readonly`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.is_property_readonly "bpy.types.bpy_struct.is_property_readonly")
  * [`bpy_struct.is_property_set`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.is_property_set "bpy.types.bpy_struct.is_property_set")
  * [`bpy_struct.items`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.items "bpy.types.bpy_struct.items")

| 

  * [`bpy_struct.keyframe_delete`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.keyframe_delete "bpy.types.bpy_struct.keyframe_delete")
  * [`bpy_struct.keyframe_insert`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.keyframe_insert "bpy.types.bpy_struct.keyframe_insert")
  * [`bpy_struct.keys`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.keys "bpy.types.bpy_struct.keys")
  * [`bpy_struct.path_from_id`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.path_from_id "bpy.types.bpy_struct.path_from_id")
  * [`bpy_struct.path_resolve`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.path_resolve "bpy.types.bpy_struct.path_resolve")
  * [`bpy_struct.pop`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.pop "bpy.types.bpy_struct.pop")
  * [`bpy_struct.property_overridable_library_set`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.property_overridable_library_set "bpy.types.bpy_struct.property_overridable_library_set")
  * [`bpy_struct.property_unset`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.property_unset "bpy.types.bpy_struct.property_unset")
  * [`bpy_struct.rna_ancestors`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.rna_ancestors "bpy.types.bpy_struct.rna_ancestors")
  * [`bpy_struct.type_recast`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.type_recast "bpy.types.bpy_struct.type_recast")
  * [`bpy_struct.values`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.values "bpy.types.bpy_struct.values")

  
---|---  
  
## References

  * [`Mesh.uv_layer_clone`](bpy.types.Mesh.html#bpy.types.Mesh.uv_layer_clone "bpy.types.Mesh.uv_layer_clone")
  * [`Mesh.uv_layer_stencil`](bpy.types.Mesh.html#bpy.types.Mesh.uv_layer_stencil "bpy.types.Mesh.uv_layer_stencil")
  * [`Mesh.uv_layers`](bpy.types.Mesh.html#bpy.types.Mesh.uv_layers "bpy.types.Mesh.uv_layers")

| 

  * [`UVLoopLayers.active`](bpy.types.UVLoopLayers.html#bpy.types.UVLoopLayers.active "bpy.types.UVLoopLayers.active")
  * [`UVLoopLayers.new`](bpy.types.UVLoopLayers.html#bpy.types.UVLoopLayers.new "bpy.types.UVLoopLayers.new")
  * [`UVLoopLayers.remove`](bpy.types.UVLoopLayers.html#bpy.types.UVLoopLayers.remove "bpy.types.UVLoopLayers.remove")

  
---|---
