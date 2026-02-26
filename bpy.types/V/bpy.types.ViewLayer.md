# ViewLayer(bpy_struct)

base class — [`bpy_struct`](bpy.types.bpy_struct.html#bpy.types.bpy_struct "bpy.types.bpy_struct")

_class _bpy.types.ViewLayer(_bpy_struct_)
    

View layer

active_aov
    

Active AOV

Type:
    

[`AOV`](bpy.types.AOV.html#bpy.types.AOV "bpy.types.AOV"), (readonly)

active_aov_index
    

Index of active AOV

Type:
    

int in [0, inf], default 0

active_layer_collection
    

Active layer collection in this view layer’s hierarchy

Type:
    

[`LayerCollection`](bpy.types.LayerCollection.html#bpy.types.LayerCollection "bpy.types.LayerCollection"), (never None)

active_lightgroup
    

Active Lightgroup

Type:
    

[`Lightgroup`](bpy.types.Lightgroup.html#bpy.types.Lightgroup "bpy.types.Lightgroup"), (readonly)

active_lightgroup_index
    

Index of active lightgroup

Type:
    

int in [0, inf], default 0

aovs
    

Type:
    

[`AOVs`](bpy.types.AOVs.html#bpy.types.AOVs "bpy.types.AOVs") [`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`AOV`](bpy.types.AOV.html#bpy.types.AOV "bpy.types.AOV"), (readonly)

cycles
    

Cycles ViewLayer Settings

Type:
    

`CyclesRenderLayerSettings`, (readonly)

depsgraph
    

Dependencies in the scene data

Type:
    

[`Depsgraph`](bpy.types.Depsgraph.html#bpy.types.Depsgraph "bpy.types.Depsgraph"), (readonly)

eevee
    

View layer settings for EEVEE

Type:
    

[`ViewLayerEEVEE`](bpy.types.ViewLayerEEVEE.html#bpy.types.ViewLayerEEVEE "bpy.types.ViewLayerEEVEE"), (readonly, never None)

freestyle_settings
    

Type:
    

[`FreestyleSettings`](bpy.types.FreestyleSettings.html#bpy.types.FreestyleSettings "bpy.types.FreestyleSettings"), (readonly, never None)

has_export_collections
    

At least one Collection in this View Layer has an exporter

Type:
    

boolean, default False, (readonly)

layer_collection
    

Root of collections hierarchy of this view layer, its ‘collection’ pointer property is the same as the scene’s master collection

Type:
    

[`LayerCollection`](bpy.types.LayerCollection.html#bpy.types.LayerCollection "bpy.types.LayerCollection"), (readonly, never None)

lightgroups
    

Type:
    

[`Lightgroups`](bpy.types.Lightgroups.html#bpy.types.Lightgroups "bpy.types.Lightgroups") [`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`Lightgroup`](bpy.types.Lightgroup.html#bpy.types.Lightgroup "bpy.types.Lightgroup"), (readonly)

material_override
    

Material to override all other materials in this view layer

Type:
    

[`Material`](bpy.types.Material.html#bpy.types.Material "bpy.types.Material")

name
    

View layer name

Type:
    

string, default “”, (never None)

objects
    

All the objects in this layer

Type:
    

[`LayerObjects`](bpy.types.LayerObjects.html#bpy.types.LayerObjects "bpy.types.LayerObjects") [`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`Object`](bpy.types.Object.html#bpy.types.Object "bpy.types.Object"), (readonly)

pass_alpha_threshold
    

Z, Index, normal, UV and vector passes are only affected by surfaces with alpha transparency equal to or higher than this threshold

Type:
    

float in [0, 1], default 0.0

pass_cryptomatte_depth
    

Sets how many unique objects can be distinguished per pixel

Type:
    

int in [2, 16], default 6

samples
    

Override number of render samples for this view layer, 0 will use the scene setting

Type:
    

int in [0, inf], default 0

use
    

Enable or disable rendering of this View Layer

Type:
    

boolean, default False

use_ao
    

Render Ambient Occlusion in this Layer

Type:
    

boolean, default False

use_freestyle
    

Render stylized strokes in this Layer

Type:
    

boolean, default False

use_grease_pencil
    

Render Grease Pencil on this layer

Type:
    

boolean, default False

use_motion_blur
    

Render motion blur in this Layer, if enabled in the scene

Type:
    

boolean, default False

use_pass_ambient_occlusion
    

Deliver Ambient Occlusion pass

Type:
    

boolean, default False

use_pass_combined
    

Deliver full combined RGBA buffer

Type:
    

boolean, default False

use_pass_cryptomatte_accurate
    

Generate a more accurate cryptomatte pass

Type:
    

boolean, default True

use_pass_cryptomatte_asset
    

Render cryptomatte asset pass, for isolating groups of objects with the same parent

Type:
    

boolean, default False

use_pass_cryptomatte_material
    

Render cryptomatte material pass, for isolating materials in compositing

Type:
    

boolean, default False

use_pass_cryptomatte_object
    

Render cryptomatte object pass, for isolating objects in compositing

Type:
    

boolean, default False

use_pass_diffuse_color
    

Deliver diffuse color pass

Type:
    

boolean, default False

use_pass_diffuse_direct
    

Deliver diffuse direct pass

Type:
    

boolean, default False

use_pass_diffuse_indirect
    

Deliver diffuse indirect pass

Type:
    

boolean, default False

use_pass_emit
    

Deliver emission pass

Type:
    

boolean, default False

use_pass_environment
    

Deliver environment lighting pass

Type:
    

boolean, default False

use_pass_glossy_color
    

Deliver glossy color pass

Type:
    

boolean, default False

use_pass_glossy_direct
    

Deliver glossy direct pass

Type:
    

boolean, default False

use_pass_glossy_indirect
    

Deliver glossy indirect pass

Type:
    

boolean, default False

use_pass_grease_pencil
    

Deliver Grease Pencil render result in a separate pass

Type:
    

boolean, default False

use_pass_material_index
    

Deliver material index pass

Type:
    

boolean, default False

use_pass_mist
    

Deliver mist factor pass (0.0 to 1.0)

Type:
    

boolean, default False

use_pass_normal
    

Deliver normal pass

Type:
    

boolean, default False

use_pass_object_index
    

Deliver object index pass

Type:
    

boolean, default False

use_pass_position
    

Deliver position pass

Type:
    

boolean, default False

use_pass_shadow
    

Deliver shadow pass

Type:
    

boolean, default False

use_pass_subsurface_color
    

Deliver subsurface color pass

Type:
    

boolean, default False

use_pass_subsurface_direct
    

Deliver subsurface direct pass

Type:
    

boolean, default False

use_pass_subsurface_indirect
    

Deliver subsurface indirect pass

Type:
    

boolean, default False

use_pass_transmission_color
    

Deliver transmission color pass

Type:
    

boolean, default False

use_pass_transmission_direct
    

Deliver transmission direct pass

Type:
    

boolean, default False

use_pass_transmission_indirect
    

Deliver transmission indirect pass

Type:
    

boolean, default False

use_pass_uv
    

Deliver texture UV pass

Type:
    

boolean, default False

use_pass_vector
    

Deliver speed vector pass

Type:
    

boolean, default False

use_pass_z
    

Deliver Z values pass

Type:
    

boolean, default False

use_sky
    

Render Sky in this Layer

Type:
    

boolean, default False

use_solid
    

Render Solid faces in this Layer

Type:
    

boolean, default False

use_strand
    

Render Strands in this Layer

Type:
    

boolean, default False

use_volumes
    

Render volumes in this Layer

Type:
    

boolean, default False

world_override
    

Override world in this view layer

Type:
    

[`World`](bpy.types.World.html#bpy.types.World "bpy.types.World")

_classmethod _update_render_passes()
    

Requery the enabled render passes from the render engine

update()
    

Update data tagged to be updated from previous access to data or operators

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

  * [`bpy.context.view_layer`](bpy.context.html#bpy.context.view_layer "bpy.context.view_layer")
  * [`Context.view_layer`](bpy.types.Context.html#bpy.types.Context.view_layer "bpy.types.Context.view_layer")
  * [`Depsgraph.view_layer`](bpy.types.Depsgraph.html#bpy.types.Depsgraph.view_layer "bpy.types.Depsgraph.view_layer")
  * [`Depsgraph.view_layer_eval`](bpy.types.Depsgraph.html#bpy.types.Depsgraph.view_layer_eval "bpy.types.Depsgraph.view_layer_eval")
  * [`ID.override_hierarchy_create`](bpy.types.ID.html#bpy.types.ID.override_hierarchy_create "bpy.types.ID.override_hierarchy_create")
  * [`IDOverrideLibrary.resync`](bpy.types.IDOverrideLibrary.html#bpy.types.IDOverrideLibrary.resync "bpy.types.IDOverrideLibrary.resync")
  * [`LayerCollection.has_selected_objects`](bpy.types.LayerCollection.html#bpy.types.LayerCollection.has_selected_objects "bpy.types.LayerCollection.has_selected_objects")
  * [`Object.hide_get`](bpy.types.Object.html#bpy.types.Object.hide_get "bpy.types.Object.hide_get")
  * [`Object.hide_set`](bpy.types.Object.html#bpy.types.Object.hide_set "bpy.types.Object.hide_set")
  * [`Object.holdout_get`](bpy.types.Object.html#bpy.types.Object.holdout_get "bpy.types.Object.holdout_get")
  * [`Object.indirect_only_get`](bpy.types.Object.html#bpy.types.Object.indirect_only_get "bpy.types.Object.indirect_only_get")

| 

  * [`Object.select_get`](bpy.types.Object.html#bpy.types.Object.select_get "bpy.types.Object.select_get")
  * [`Object.select_set`](bpy.types.Object.html#bpy.types.Object.select_set "bpy.types.Object.select_set")
  * [`Object.visible_get`](bpy.types.Object.html#bpy.types.Object.visible_get "bpy.types.Object.visible_get")
  * [`RenderEngine.register_pass`](bpy.types.RenderEngine.html#bpy.types.RenderEngine.register_pass "bpy.types.RenderEngine.register_pass")
  * [`RenderEngine.update_render_passes`](bpy.types.RenderEngine.html#bpy.types.RenderEngine.update_render_passes "bpy.types.RenderEngine.update_render_passes")
  * [`Scene.statistics`](bpy.types.Scene.html#bpy.types.Scene.statistics "bpy.types.Scene.statistics")
  * [`Scene.view_layers`](bpy.types.Scene.html#bpy.types.Scene.view_layers "bpy.types.Scene.view_layers")
  * [`ViewLayers.new`](bpy.types.ViewLayers.html#bpy.types.ViewLayers.new "bpy.types.ViewLayers.new")
  * [`ViewLayers.remove`](bpy.types.ViewLayers.html#bpy.types.ViewLayers.remove "bpy.types.ViewLayers.remove")
  * [`Window.view_layer`](bpy.types.Window.html#bpy.types.Window.view_layer "bpy.types.Window.view_layer")

  
---|---
