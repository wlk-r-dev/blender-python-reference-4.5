# GreasePencilv3(ID)

base classes — [`bpy_struct`](bpy.types.bpy_struct.html#bpy.types.bpy_struct "bpy.types.bpy_struct"), [`ID`](bpy.types.ID.html#bpy.types.ID "bpy.types.ID")

_class _bpy.types.GreasePencilv3(_ID_)
    

Grease Pencil data-block

after_color
    

Base color for ghosts after the active frame

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.12549, 0.082353, 0.529412)

animation_data
    

Animation data for this data-block

Type:
    

[`AnimData`](bpy.types.AnimData.html#bpy.types.AnimData "bpy.types.AnimData"), (readonly)

attributes
    

Geometry attributes

Type:
    

[`AttributeGroupGreasePencil`](bpy.types.AttributeGroupGreasePencil.html#bpy.types.AttributeGroupGreasePencil "bpy.types.AttributeGroupGreasePencil") [`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`Attribute`](bpy.types.Attribute.html#bpy.types.Attribute "bpy.types.Attribute"), (readonly)

before_color
    

Base color for ghosts before the active frame

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.145098, 0.419608, 0.137255)

color_attributes
    

Geometry color attributes

Type:
    

[`AttributeGroupGreasePencil`](bpy.types.AttributeGroupGreasePencil.html#bpy.types.AttributeGroupGreasePencil "bpy.types.AttributeGroupGreasePencil") [`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`Attribute`](bpy.types.Attribute.html#bpy.types.Attribute "bpy.types.Attribute"), (readonly)

ghost_after_range
    

Maximum number of frames to show after current frame (0 = don’t show any frames after current)

Type:
    

int in [0, 120], default 1

ghost_before_range
    

Maximum number of frames to show before current frame (0 = don’t show any frames before current)

Type:
    

int in [0, 120], default 1

layer_groups
    

Grease Pencil layer groups

Type:
    

[`GreasePencilv3LayerGroup`](bpy.types.GreasePencilv3LayerGroup.html#bpy.types.GreasePencilv3LayerGroup "bpy.types.GreasePencilv3LayerGroup") [`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`GreasePencilLayerGroup`](bpy.types.GreasePencilLayerGroup.html#bpy.types.GreasePencilLayerGroup "bpy.types.GreasePencilLayerGroup"), (readonly)

layers
    

Grease Pencil layers

Type:
    

[`GreasePencilv3Layers`](bpy.types.GreasePencilv3Layers.html#bpy.types.GreasePencilv3Layers "bpy.types.GreasePencilv3Layers") [`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`GreasePencilLayer`](bpy.types.GreasePencilLayer.html#bpy.types.GreasePencilLayer "bpy.types.GreasePencilLayer"), (readonly)

materials
    

Type:
    

[`IDMaterials`](bpy.types.IDMaterials.html#bpy.types.IDMaterials "bpy.types.IDMaterials") [`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`Material`](bpy.types.Material.html#bpy.types.Material "bpy.types.Material"), (readonly)

onion_factor
    

Change fade opacity of displayed onion frames

Type:
    

float in [0, 1], default 0.5

onion_keyframe_type
    

Type of keyframe (for filtering)

  * `ALL` All – Include all Keyframe types.

  * `KEYFRAME` Keyframe – Normal keyframe, e.g. for key poses.

  * `BREAKDOWN` Breakdown – A breakdown pose, e.g. for transitions between key poses.

  * `MOVING_HOLD` Moving Hold – A keyframe that is part of a moving hold.

  * `EXTREME` Extreme – An ‘extreme’ pose, or some other purpose as needed.

  * `JITTER` Jitter – A filler or baked keyframe for keying on ones, or some other purpose as needed.

  * `GENERATED` Generated – A key generated automatically by a tool, not manually created.


Type:
    

enum in [`'ALL'`, `'KEYFRAME'`, `'BREAKDOWN'`, `'MOVING_HOLD'`, `'EXTREME'`, `'JITTER'`, `'GENERATED'`], default `'ALL'`

onion_mode
    

Mode to display frames

  * `ABSOLUTE` Frames – Frames in absolute range of the scene frame.

  * `RELATIVE` Keyframes – Frames in relative range of the Grease Pencil keyframes.

  * `SELECTED` Selected – Only selected keyframes.


Type:
    

enum in [`'ABSOLUTE'`, `'RELATIVE'`, `'SELECTED'`], default `'ABSOLUTE'`

stroke_depth_order
    

Defines how the strokes are ordered in 3D space (for objects not displayed ‘In Front’)

Type:
    

enum in [Stroke Depth Order Items](bpy_types_enum_items/stroke_depth_order_items.html#rna-enum-stroke-depth-order-items), default `'2D'`

use_autolock_layers
    

Automatically lock all layers except the active one to avoid accidental changes

Type:
    

boolean, default False

use_ghost_custom_colors
    

Use custom colors for ghost frames

Type:
    

boolean, default False

use_onion_fade
    

Display onion keyframes with a fade in color transparency

Type:
    

boolean, default False

use_onion_loop
    

Display onion keyframes for looping animations

Type:
    

boolean, default False

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
  * [`ID.name`](bpy.types.ID.html#bpy.types.ID.name "bpy.types.ID.name")
  * [`ID.name_full`](bpy.types.ID.html#bpy.types.ID.name_full "bpy.types.ID.name_full")
  * [`ID.id_type`](bpy.types.ID.html#bpy.types.ID.id_type "bpy.types.ID.id_type")
  * [`ID.session_uid`](bpy.types.ID.html#bpy.types.ID.session_uid "bpy.types.ID.session_uid")
  * [`ID.is_evaluated`](bpy.types.ID.html#bpy.types.ID.is_evaluated "bpy.types.ID.is_evaluated")
  * [`ID.original`](bpy.types.ID.html#bpy.types.ID.original "bpy.types.ID.original")
  * [`ID.users`](bpy.types.ID.html#bpy.types.ID.users "bpy.types.ID.users")
  * [`ID.use_fake_user`](bpy.types.ID.html#bpy.types.ID.use_fake_user "bpy.types.ID.use_fake_user")
  * [`ID.use_extra_user`](bpy.types.ID.html#bpy.types.ID.use_extra_user "bpy.types.ID.use_extra_user")
  * [`ID.is_embedded_data`](bpy.types.ID.html#bpy.types.ID.is_embedded_data "bpy.types.ID.is_embedded_data")

| 

  * [`ID.is_missing`](bpy.types.ID.html#bpy.types.ID.is_missing "bpy.types.ID.is_missing")
  * [`ID.is_runtime_data`](bpy.types.ID.html#bpy.types.ID.is_runtime_data "bpy.types.ID.is_runtime_data")
  * [`ID.is_editable`](bpy.types.ID.html#bpy.types.ID.is_editable "bpy.types.ID.is_editable")
  * [`ID.tag`](bpy.types.ID.html#bpy.types.ID.tag "bpy.types.ID.tag")
  * [`ID.is_library_indirect`](bpy.types.ID.html#bpy.types.ID.is_library_indirect "bpy.types.ID.is_library_indirect")
  * [`ID.library`](bpy.types.ID.html#bpy.types.ID.library "bpy.types.ID.library")
  * [`ID.library_weak_reference`](bpy.types.ID.html#bpy.types.ID.library_weak_reference "bpy.types.ID.library_weak_reference")
  * [`ID.asset_data`](bpy.types.ID.html#bpy.types.ID.asset_data "bpy.types.ID.asset_data")
  * [`ID.override_library`](bpy.types.ID.html#bpy.types.ID.override_library "bpy.types.ID.override_library")
  * [`ID.preview`](bpy.types.ID.html#bpy.types.ID.preview "bpy.types.ID.preview")

  
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
  * [`bpy_struct.keyframe_delete`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.keyframe_delete "bpy.types.bpy_struct.keyframe_delete")
  * [`bpy_struct.keyframe_insert`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.keyframe_insert "bpy.types.bpy_struct.keyframe_insert")
  * [`bpy_struct.keys`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.keys "bpy.types.bpy_struct.keys")
  * [`bpy_struct.path_from_id`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.path_from_id "bpy.types.bpy_struct.path_from_id")
  * [`bpy_struct.path_resolve`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.path_resolve "bpy.types.bpy_struct.path_resolve")
  * [`bpy_struct.pop`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.pop "bpy.types.bpy_struct.pop")
  * [`bpy_struct.property_overridable_library_set`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.property_overridable_library_set "bpy.types.bpy_struct.property_overridable_library_set")
  * [`bpy_struct.property_unset`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.property_unset "bpy.types.bpy_struct.property_unset")
  * [`bpy_struct.rna_ancestors`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.rna_ancestors "bpy.types.bpy_struct.rna_ancestors")

| 

  * [`bpy_struct.type_recast`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.type_recast "bpy.types.bpy_struct.type_recast")
  * [`bpy_struct.values`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.values "bpy.types.bpy_struct.values")
  * [`ID.rename`](bpy.types.ID.html#bpy.types.ID.rename "bpy.types.ID.rename")
  * [`ID.evaluated_get`](bpy.types.ID.html#bpy.types.ID.evaluated_get "bpy.types.ID.evaluated_get")
  * [`ID.copy`](bpy.types.ID.html#bpy.types.ID.copy "bpy.types.ID.copy")
  * [`ID.asset_mark`](bpy.types.ID.html#bpy.types.ID.asset_mark "bpy.types.ID.asset_mark")
  * [`ID.asset_clear`](bpy.types.ID.html#bpy.types.ID.asset_clear "bpy.types.ID.asset_clear")
  * [`ID.asset_generate_preview`](bpy.types.ID.html#bpy.types.ID.asset_generate_preview "bpy.types.ID.asset_generate_preview")
  * [`ID.override_create`](bpy.types.ID.html#bpy.types.ID.override_create "bpy.types.ID.override_create")
  * [`ID.override_hierarchy_create`](bpy.types.ID.html#bpy.types.ID.override_hierarchy_create "bpy.types.ID.override_hierarchy_create")
  * [`ID.user_clear`](bpy.types.ID.html#bpy.types.ID.user_clear "bpy.types.ID.user_clear")
  * [`ID.user_remap`](bpy.types.ID.html#bpy.types.ID.user_remap "bpy.types.ID.user_remap")
  * [`ID.make_local`](bpy.types.ID.html#bpy.types.ID.make_local "bpy.types.ID.make_local")
  * [`ID.user_of_id`](bpy.types.ID.html#bpy.types.ID.user_of_id "bpy.types.ID.user_of_id")
  * [`ID.animation_data_create`](bpy.types.ID.html#bpy.types.ID.animation_data_create "bpy.types.ID.animation_data_create")
  * [`ID.animation_data_clear`](bpy.types.ID.html#bpy.types.ID.animation_data_clear "bpy.types.ID.animation_data_clear")
  * [`ID.update_tag`](bpy.types.ID.html#bpy.types.ID.update_tag "bpy.types.ID.update_tag")
  * [`ID.preview_ensure`](bpy.types.ID.html#bpy.types.ID.preview_ensure "bpy.types.ID.preview_ensure")
  * [`ID.bl_rna_get_subclass`](bpy.types.ID.html#bpy.types.ID.bl_rna_get_subclass "bpy.types.ID.bl_rna_get_subclass")
  * [`ID.bl_rna_get_subclass_py`](bpy.types.ID.html#bpy.types.ID.bl_rna_get_subclass_py "bpy.types.ID.bl_rna_get_subclass_py")

  
---|---  
  
## References

  * [`bpy.context.grease_pencil`](bpy.context.html#bpy.context.grease_pencil "bpy.context.grease_pencil")
  * [`BlendData.grease_pencils_v3`](bpy.types.BlendData.html#bpy.types.BlendData.grease_pencils_v3 "bpy.types.BlendData.grease_pencils_v3")

| 

  * [`BlendDataGreasePencilsV3.new`](bpy.types.BlendDataGreasePencilsV3.html#bpy.types.BlendDataGreasePencilsV3.new "bpy.types.BlendDataGreasePencilsV3.new")
  * [`BlendDataGreasePencilsV3.remove`](bpy.types.BlendDataGreasePencilsV3.html#bpy.types.BlendDataGreasePencilsV3.remove "bpy.types.BlendDataGreasePencilsV3.remove")

  
---|---
