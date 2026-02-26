# PreferencesExperimental(bpy_struct)

base class — [`bpy_struct`](bpy.types.bpy_struct.md#bpy.types.bpy_struct "bpy.types.bpy_struct")

_class _bpy.types.PreferencesExperimental(_bpy_struct_)
    

Experimental features

override_auto_resync
    

Disable library overrides automatic resync detection and process on file load (can be useful to help fixing broken files). Also see the –disable-liboverride-auto-resync command line option

Type:
    

boolean, default False

show_asset_debug_info
    

Enable some extra fields in the Asset Browser to aid in debugging

Type:
    

boolean, default False

use_all_linked_data_direct
    

Forces all linked data to be considered as directly linked. Workaround for current issues/limitations in BAT (Blender studio pipeline tool)

Type:
    

boolean, default False

use_asset_indexing
    

Disable the asset indexer, to force every asset library refresh to completely reread assets from disk

Type:
    

boolean, default False

use_attribute_storage_write
    

Instead of writing with the older “CustomData” format for forward compatibility, use the new “AttributeStorage” format

Type:
    

boolean, default False

use_bundle_and_closure_nodes
    

Enables bundle and closure nodes in Geometry Nodes

Type:
    

boolean, default False

use_cycles_debug
    

Enable Cycles debugging options for developers

Type:
    

boolean, default False

use_eevee_debug
    

Enable EEVEE debugging options for developers

Type:
    

boolean, default False

use_extended_asset_browser
    

Enable Asset Browser editor and operators to manage regular data-blocks as assets, not just poses

Type:
    

boolean, default False

use_extensions_debug
    

Extra debugging information & developer support utilities for extensions

Type:
    

boolean, default False

use_new_curves_tools
    

Enable additional features for the new curves data block

Type:
    

boolean, default False

use_new_volume_nodes
    

Enables visibility of the new Volume nodes in the UI

Type:
    

boolean, default False

use_recompute_usercount_on_save_debug
    

Recompute all ID usercounts before saving to a blendfile. Allows to work around invalid usercount handling in code that may lead to loss of data due to wrongly detected unused data-blocks

Type:
    

boolean, default False

use_sculpt_texture_paint
    

Use texture painting in Sculpt Mode

Type:
    

boolean, default False

use_shader_node_previews
    

Enables previews in the shader node editor

Type:
    

boolean, default False

use_socket_structure_type
    

Enables new visualization of socket data compatibility in Geometry Nodes

Type:
    

boolean, default False

use_undo_legacy
    

Use legacy undo (slower than the new default one, but may be more stable in some cases)

Type:
    

boolean, default False

use_viewport_debug
    

Enable viewport debugging options for developers in the overlays pop-over

Type:
    

boolean, default False

write_large_blend_file_blocks
    

Enables support for writing .blend files that contain buffers larger than 2 GB. If enabled, any saved files can not be opened by older Blender versions

Type:
    

boolean, default False

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

## Inherited Properties

  * [`bpy_struct.id_data`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.id_data "bpy.types.bpy_struct.id_data")

| 


  
---|---  
  
## Inherited Functions

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
  
## References

  * [`Preferences.experimental`](bpy.types.Preferences.md#bpy.types.Preferences.experimental "bpy.types.Preferences.experimental")

| 


  
---|---
