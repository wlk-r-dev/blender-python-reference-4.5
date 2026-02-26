# ThemeClipEditor(bpy_struct)

base class — [`bpy_struct`](bpy.types.bpy_struct.html#bpy.types.bpy_struct "bpy.types.bpy_struct")

_class _bpy.types.ThemeClipEditor(_bpy_struct_)
    

Theme settings for the Movie Clip Editor

active_marker
    

Color of active marker

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

disabled_marker
    

Color of disabled marker

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

frame_current
    

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

grid
    

Type:
    

float array of 4 items in [0, 1], default (0.0, 0.0, 0.0, 0.0)

handle_align
    

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

handle_auto
    

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

handle_auto_clamped
    

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

handle_free
    

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

handle_sel_align
    

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

handle_sel_auto
    

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

handle_sel_auto_clamped
    

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

handle_sel_free
    

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

handle_vertex
    

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

handle_vertex_select
    

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

handle_vertex_size
    

Type:
    

int in [1, 100], default 0

locked_marker
    

Color of locked marker

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

marker
    

Color of marker

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

marker_outline
    

Color of marker’s outline

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

metadatabg
    

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

metadatatext
    

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

path_after
    

Color of path after current frame

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

path_before
    

Color of path before current frame

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

path_keyframe_after
    

Color of keyframes on a path after current frame

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

path_keyframe_before
    

Color of keyframes on a path before current frame

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

preview_range
    

Color of preview range overlay

Type:
    

float array of 4 items in [0, 1], default (0.0, 0.0, 0.0, 0.0)

selected_marker
    

Color of selected marker

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

space
    

Settings for space

Type:
    

[`ThemeSpaceGeneric`](bpy.types.ThemeSpaceGeneric.html#bpy.types.ThemeSpaceGeneric "bpy.types.ThemeSpaceGeneric"), (readonly, never None)

space_list
    

Settings for space list

Type:
    

[`ThemeSpaceListGeneric`](bpy.types.ThemeSpaceListGeneric.html#bpy.types.ThemeSpaceListGeneric "bpy.types.ThemeSpaceListGeneric"), (readonly, never None)

strips
    

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

strips_selected
    

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

time_marker_line
    

Type:
    

float array of 4 items in [0, 1], default (0.0, 0.0, 0.0, 0.0)

time_marker_line_selected
    

Type:
    

float array of 4 items in [0, 1], default (0.0, 0.0, 0.0, 0.0)

time_scrub_background
    

Type:
    

float array of 4 items in [0, 1], default (0.0, 0.0, 0.0, 0.0)

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

  * [`Theme.clip_editor`](bpy.types.Theme.html#bpy.types.Theme.clip_editor "bpy.types.Theme.clip_editor")

| 


  
---|---
