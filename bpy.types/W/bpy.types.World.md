# World(ID)

base classes — [`bpy_struct`](bpy.types.bpy_struct.md#bpy.types.bpy_struct "bpy.types.bpy_struct"), [`ID`](bpy.types.ID.md#bpy.types.ID "bpy.types.ID")

_class _bpy.types.World(_ID_)
    

World data-block describing the environment and ambient lighting of a scene

animation_data
    

Animation data for this data-block

Type:
    

[`AnimData`](bpy.types.AnimData.md#bpy.types.AnimData "bpy.types.AnimData"), (readonly)

color
    

Color of the background

Type:
    

[`mathutils.Color`](mathutils.md#mathutils.Color "mathutils.Color") of 3 items in [0, inf], default (0.05, 0.05, 0.05)

cycles
    

Cycles world settings

Type:
    

`CyclesWorldSettings`, (readonly)

cycles_visibility
    

Cycles visibility settings

Type:
    

`CyclesVisibilitySettings`, (readonly)

light_settings
    

World lighting settings

Type:
    

[`WorldLighting`](bpy.types.WorldLighting.md#bpy.types.WorldLighting "bpy.types.WorldLighting"), (readonly, never None)

lightgroup
    

Lightgroup that the world belongs to

Type:
    

string, default “”, (never None)

mist_settings
    

World mist settings

Type:
    

[`WorldMistSettings`](bpy.types.WorldMistSettings.md#bpy.types.WorldMistSettings "bpy.types.WorldMistSettings"), (readonly, never None)

node_tree
    

Node tree for node based worlds

Type:
    

[`NodeTree`](bpy.types.NodeTree.md#bpy.types.NodeTree "bpy.types.NodeTree"), (readonly)

probe_resolution
    

Resolution when baked to a texture

Type:
    

enum in [`'128'`, `'256'`, `'512'`, `'1024'`, `'2048'`, `'4096'`], default `'1024'`

sun_angle
    

Angular diameter of the Sun as seen from the Earth

Type:
    

float in [0, 3.14159], default 0.00918043

sun_shadow_filter_radius
    

Blur shadow aliasing using Percentage Closer Filtering

Type:
    

float in [0, inf], default 1.0

sun_shadow_jitter_overblur
    

Apply shadow tracing to each jittered sample to reduce under-sampling artifacts

Type:
    

float in [0, 100], default 10.0

sun_shadow_maximum_resolution
    

Maximum size of a shadow map pixel. Higher values use less memory at the cost of shadow quality.

Type:
    

float in [0, inf], default 0.001

sun_threshold
    

If non-zero, the maximum value for world contribution that will be recorded inside the world light probe. The excess contribution is converted to a sun light. This reduces the light bleeding caused by very bright light sources.

Type:
    

float in [0, inf], default 10.0

use_eevee_finite_volume
    

The world’s volume used to be rendered by EEVEE Legacy. Conversion is needed for it to render properly.

Type:
    

boolean, default False

use_nodes
    

Use shader nodes to render the world

Type:
    

boolean, default False

use_sun_shadow
    

Enable sun shadow casting

Type:
    

boolean, default True

use_sun_shadow_jitter
    

Enable jittered soft shadows to increase shadow precision (disabled in viewport unless enabled in the render settings). Has a high performance impact.

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
  * [`ID.name`](bpy.types.ID.md#bpy.types.ID.name "bpy.types.ID.name")
  * [`ID.name_full`](bpy.types.ID.md#bpy.types.ID.name_full "bpy.types.ID.name_full")
  * [`ID.id_type`](bpy.types.ID.md#bpy.types.ID.id_type "bpy.types.ID.id_type")
  * [`ID.session_uid`](bpy.types.ID.md#bpy.types.ID.session_uid "bpy.types.ID.session_uid")
  * [`ID.is_evaluated`](bpy.types.ID.md#bpy.types.ID.is_evaluated "bpy.types.ID.is_evaluated")
  * [`ID.original`](bpy.types.ID.md#bpy.types.ID.original "bpy.types.ID.original")
  * [`ID.users`](bpy.types.ID.md#bpy.types.ID.users "bpy.types.ID.users")
  * [`ID.use_fake_user`](bpy.types.ID.md#bpy.types.ID.use_fake_user "bpy.types.ID.use_fake_user")
  * [`ID.use_extra_user`](bpy.types.ID.md#bpy.types.ID.use_extra_user "bpy.types.ID.use_extra_user")
  * [`ID.is_embedded_data`](bpy.types.ID.md#bpy.types.ID.is_embedded_data "bpy.types.ID.is_embedded_data")

| 

  * [`ID.is_missing`](bpy.types.ID.md#bpy.types.ID.is_missing "bpy.types.ID.is_missing")
  * [`ID.is_runtime_data`](bpy.types.ID.md#bpy.types.ID.is_runtime_data "bpy.types.ID.is_runtime_data")
  * [`ID.is_editable`](bpy.types.ID.md#bpy.types.ID.is_editable "bpy.types.ID.is_editable")
  * [`ID.tag`](bpy.types.ID.md#bpy.types.ID.tag "bpy.types.ID.tag")
  * [`ID.is_library_indirect`](bpy.types.ID.md#bpy.types.ID.is_library_indirect "bpy.types.ID.is_library_indirect")
  * [`ID.library`](bpy.types.ID.md#bpy.types.ID.library "bpy.types.ID.library")
  * [`ID.library_weak_reference`](bpy.types.ID.md#bpy.types.ID.library_weak_reference "bpy.types.ID.library_weak_reference")
  * [`ID.asset_data`](bpy.types.ID.md#bpy.types.ID.asset_data "bpy.types.ID.asset_data")
  * [`ID.override_library`](bpy.types.ID.md#bpy.types.ID.override_library "bpy.types.ID.override_library")
  * [`ID.preview`](bpy.types.ID.md#bpy.types.ID.preview "bpy.types.ID.preview")

  
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
  * [`bpy_struct.keyframe_delete`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.keyframe_delete "bpy.types.bpy_struct.keyframe_delete")
  * [`bpy_struct.keyframe_insert`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.keyframe_insert "bpy.types.bpy_struct.keyframe_insert")
  * [`bpy_struct.keys`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.keys "bpy.types.bpy_struct.keys")
  * [`bpy_struct.path_from_id`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.path_from_id "bpy.types.bpy_struct.path_from_id")
  * [`bpy_struct.path_resolve`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.path_resolve "bpy.types.bpy_struct.path_resolve")
  * [`bpy_struct.pop`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.pop "bpy.types.bpy_struct.pop")
  * [`bpy_struct.property_overridable_library_set`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.property_overridable_library_set "bpy.types.bpy_struct.property_overridable_library_set")
  * [`bpy_struct.property_unset`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.property_unset "bpy.types.bpy_struct.property_unset")
  * [`bpy_struct.rna_ancestors`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.rna_ancestors "bpy.types.bpy_struct.rna_ancestors")

| 

  * [`bpy_struct.type_recast`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.type_recast "bpy.types.bpy_struct.type_recast")
  * [`bpy_struct.values`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.values "bpy.types.bpy_struct.values")
  * [`ID.rename`](bpy.types.ID.md#bpy.types.ID.rename "bpy.types.ID.rename")
  * [`ID.evaluated_get`](bpy.types.ID.md#bpy.types.ID.evaluated_get "bpy.types.ID.evaluated_get")
  * [`ID.copy`](bpy.types.ID.md#bpy.types.ID.copy "bpy.types.ID.copy")
  * [`ID.asset_mark`](bpy.types.ID.md#bpy.types.ID.asset_mark "bpy.types.ID.asset_mark")
  * [`ID.asset_clear`](bpy.types.ID.md#bpy.types.ID.asset_clear "bpy.types.ID.asset_clear")
  * [`ID.asset_generate_preview`](bpy.types.ID.md#bpy.types.ID.asset_generate_preview "bpy.types.ID.asset_generate_preview")
  * [`ID.override_create`](bpy.types.ID.md#bpy.types.ID.override_create "bpy.types.ID.override_create")
  * [`ID.override_hierarchy_create`](bpy.types.ID.md#bpy.types.ID.override_hierarchy_create "bpy.types.ID.override_hierarchy_create")
  * [`ID.user_clear`](bpy.types.ID.md#bpy.types.ID.user_clear "bpy.types.ID.user_clear")
  * [`ID.user_remap`](bpy.types.ID.md#bpy.types.ID.user_remap "bpy.types.ID.user_remap")
  * [`ID.make_local`](bpy.types.ID.md#bpy.types.ID.make_local "bpy.types.ID.make_local")
  * [`ID.user_of_id`](bpy.types.ID.md#bpy.types.ID.user_of_id "bpy.types.ID.user_of_id")
  * [`ID.animation_data_create`](bpy.types.ID.md#bpy.types.ID.animation_data_create "bpy.types.ID.animation_data_create")
  * [`ID.animation_data_clear`](bpy.types.ID.md#bpy.types.ID.animation_data_clear "bpy.types.ID.animation_data_clear")
  * [`ID.update_tag`](bpy.types.ID.md#bpy.types.ID.update_tag "bpy.types.ID.update_tag")
  * [`ID.preview_ensure`](bpy.types.ID.md#bpy.types.ID.preview_ensure "bpy.types.ID.preview_ensure")
  * [`ID.bl_rna_get_subclass`](bpy.types.ID.md#bpy.types.ID.bl_rna_get_subclass "bpy.types.ID.bl_rna_get_subclass")
  * [`ID.bl_rna_get_subclass_py`](bpy.types.ID.md#bpy.types.ID.bl_rna_get_subclass_py "bpy.types.ID.bl_rna_get_subclass_py")

  
---|---  
  
## References

  * [`bpy.context.world`](bpy.context.md#bpy.context.world "bpy.context.world")
  * [`BlendData.worlds`](bpy.types.BlendData.md#bpy.types.BlendData.worlds "bpy.types.BlendData.worlds")
  * [`BlendDataWorlds.new`](bpy.types.BlendDataWorlds.md#bpy.types.BlendDataWorlds.new "bpy.types.BlendDataWorlds.new")

| 

  * [`BlendDataWorlds.remove`](bpy.types.BlendDataWorlds.md#bpy.types.BlendDataWorlds.remove "bpy.types.BlendDataWorlds.remove")
  * [`Scene.world`](bpy.types.Scene.md#bpy.types.Scene.world "bpy.types.Scene.world")
  * [`ViewLayer.world_override`](bpy.types.ViewLayer.md#bpy.types.ViewLayer.world_override "bpy.types.ViewLayer.world_override")

  
---|---
