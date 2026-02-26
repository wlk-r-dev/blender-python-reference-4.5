# VIEW3D_AST_brush_gpencil_weight(AssetShelf)

base classes — [`bpy_struct`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct "bpy.types.bpy_struct"), [`AssetShelf`](../A/bpy.types.AssetShelf.md#bpy.types.AssetShelf "bpy.types.AssetShelf")

_class _bpy.types.VIEW3D_AST_brush_gpencil_weight(_AssetShelf_)
    

_classmethod _brush_type_poll(_context_ , _asset_)
    

_static _draw_popup_selector(_layout_ , _context_ , _brush_ , _show_name =True_)
    

_static _get_shelf_name_from_context(_context_)
    

_classmethod _has_tool_with_brush_type(_context_ , _brush_type_)
    

_classmethod _bl_rna_get_subclass(_id_ , _default =None_, _/_)
    

Parameters:
    

**id** (_str_) – The RNA type identifier.

Returns:
    

The RNA type or default when not found.

Return type:
    

[`bpy.types.Struct`](../S/bpy.types.Struct.md#bpy.types.Struct "bpy.types.Struct") subclass

_classmethod _bl_rna_get_subclass_py(_id_ , _default =None_, _/_)
    

Parameters:
    

**id** (_str_) – The RNA type identifier.

Returns:
    

The class or default when not found.

Return type:
    

type

## Inherited Properties

  * [`bpy_struct.id_data`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.id_data "bpy.types.bpy_struct.id_data")
  * [`AssetShelf.bl_idname`](../A/bpy.types.AssetShelf.md#bpy.types.AssetShelf.bl_idname "bpy.types.AssetShelf.bl_idname")
  * [`AssetShelf.bl_space_type`](../A/bpy.types.AssetShelf.md#bpy.types.AssetShelf.bl_space_type "bpy.types.AssetShelf.bl_space_type")
  * [`AssetShelf.bl_options`](../A/bpy.types.AssetShelf.md#bpy.types.AssetShelf.bl_options "bpy.types.AssetShelf.bl_options")
  * [`AssetShelf.bl_activate_operator`](../A/bpy.types.AssetShelf.md#bpy.types.AssetShelf.bl_activate_operator "bpy.types.AssetShelf.bl_activate_operator")

| 

  * [`AssetShelf.bl_default_preview_size`](../A/bpy.types.AssetShelf.md#bpy.types.AssetShelf.bl_default_preview_size "bpy.types.AssetShelf.bl_default_preview_size")
  * [`AssetShelf.asset_library_reference`](../A/bpy.types.AssetShelf.md#bpy.types.AssetShelf.asset_library_reference "bpy.types.AssetShelf.asset_library_reference")
  * [`AssetShelf.show_names`](../A/bpy.types.AssetShelf.md#bpy.types.AssetShelf.show_names "bpy.types.AssetShelf.show_names")
  * [`AssetShelf.preview_size`](../A/bpy.types.AssetShelf.md#bpy.types.AssetShelf.preview_size "bpy.types.AssetShelf.preview_size")
  * [`AssetShelf.search_filter`](../A/bpy.types.AssetShelf.md#bpy.types.AssetShelf.search_filter "bpy.types.AssetShelf.search_filter")

  
---|---  
  
## Inherited Functions

  * [`bpy_struct.as_pointer`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.as_pointer "bpy.types.bpy_struct.as_pointer")
  * [`bpy_struct.driver_add`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.driver_add "bpy.types.bpy_struct.driver_add")
  * [`bpy_struct.driver_remove`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.driver_remove "bpy.types.bpy_struct.driver_remove")
  * [`bpy_struct.get`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.get "bpy.types.bpy_struct.get")
  * [`bpy_struct.id_properties_clear`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.id_properties_clear "bpy.types.bpy_struct.id_properties_clear")
  * [`bpy_struct.id_properties_ensure`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.id_properties_ensure "bpy.types.bpy_struct.id_properties_ensure")
  * [`bpy_struct.id_properties_ui`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.id_properties_ui "bpy.types.bpy_struct.id_properties_ui")
  * [`bpy_struct.is_property_hidden`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.is_property_hidden "bpy.types.bpy_struct.is_property_hidden")
  * [`bpy_struct.is_property_overridable_library`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.is_property_overridable_library "bpy.types.bpy_struct.is_property_overridable_library")
  * [`bpy_struct.is_property_readonly`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.is_property_readonly "bpy.types.bpy_struct.is_property_readonly")
  * [`bpy_struct.is_property_set`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.is_property_set "bpy.types.bpy_struct.is_property_set")
  * [`bpy_struct.items`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.items "bpy.types.bpy_struct.items")
  * [`bpy_struct.keyframe_delete`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.keyframe_delete "bpy.types.bpy_struct.keyframe_delete")
  * [`bpy_struct.keyframe_insert`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.keyframe_insert "bpy.types.bpy_struct.keyframe_insert")
  * [`bpy_struct.keys`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.keys "bpy.types.bpy_struct.keys")

| 

  * [`bpy_struct.path_from_id`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.path_from_id "bpy.types.bpy_struct.path_from_id")
  * [`bpy_struct.path_resolve`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.path_resolve "bpy.types.bpy_struct.path_resolve")
  * [`bpy_struct.pop`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.pop "bpy.types.bpy_struct.pop")
  * [`bpy_struct.property_overridable_library_set`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.property_overridable_library_set "bpy.types.bpy_struct.property_overridable_library_set")
  * [`bpy_struct.property_unset`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.property_unset "bpy.types.bpy_struct.property_unset")
  * [`bpy_struct.rna_ancestors`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.rna_ancestors "bpy.types.bpy_struct.rna_ancestors")
  * [`bpy_struct.type_recast`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.type_recast "bpy.types.bpy_struct.type_recast")
  * [`bpy_struct.values`](../_other/bpy.types.bpy_struct.md#bpy.types.bpy_struct.values "bpy.types.bpy_struct.values")
  * [`AssetShelf.poll`](../A/bpy.types.AssetShelf.md#bpy.types.AssetShelf.poll "bpy.types.AssetShelf.poll")
  * [`AssetShelf.asset_poll`](../A/bpy.types.AssetShelf.md#bpy.types.AssetShelf.asset_poll "bpy.types.AssetShelf.asset_poll")
  * [`AssetShelf.get_active_asset`](../A/bpy.types.AssetShelf.md#bpy.types.AssetShelf.get_active_asset "bpy.types.AssetShelf.get_active_asset")
  * [`AssetShelf.draw_context_menu`](../A/bpy.types.AssetShelf.md#bpy.types.AssetShelf.draw_context_menu "bpy.types.AssetShelf.draw_context_menu")
  * [`AssetShelf.bl_rna_get_subclass`](../A/bpy.types.AssetShelf.md#bpy.types.AssetShelf.bl_rna_get_subclass "bpy.types.AssetShelf.bl_rna_get_subclass")
  * [`AssetShelf.bl_rna_get_subclass_py`](../A/bpy.types.AssetShelf.md#bpy.types.AssetShelf.bl_rna_get_subclass_py "bpy.types.AssetShelf.bl_rna_get_subclass_py")

  
---|---
