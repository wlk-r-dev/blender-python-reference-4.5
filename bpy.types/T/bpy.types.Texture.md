# Texture(ID)

base classes — [`bpy_struct`](bpy.types.bpy_struct.html#bpy.types.bpy_struct "bpy.types.bpy_struct"), [`ID`](bpy.types.ID.html#bpy.types.ID "bpy.types.ID")

subclasses — [`BlendTexture`](bpy.types.BlendTexture.html#bpy.types.BlendTexture "bpy.types.BlendTexture"), [`CloudsTexture`](bpy.types.CloudsTexture.html#bpy.types.CloudsTexture "bpy.types.CloudsTexture"), [`DistortedNoiseTexture`](bpy.types.DistortedNoiseTexture.html#bpy.types.DistortedNoiseTexture "bpy.types.DistortedNoiseTexture"), [`ImageTexture`](bpy.types.ImageTexture.html#bpy.types.ImageTexture "bpy.types.ImageTexture"), [`MagicTexture`](bpy.types.MagicTexture.html#bpy.types.MagicTexture "bpy.types.MagicTexture"), [`MarbleTexture`](bpy.types.MarbleTexture.html#bpy.types.MarbleTexture "bpy.types.MarbleTexture"), [`MusgraveTexture`](bpy.types.MusgraveTexture.html#bpy.types.MusgraveTexture "bpy.types.MusgraveTexture"), [`NoiseTexture`](bpy.types.NoiseTexture.html#bpy.types.NoiseTexture "bpy.types.NoiseTexture"), [`StucciTexture`](bpy.types.StucciTexture.html#bpy.types.StucciTexture "bpy.types.StucciTexture"), [`VoronoiTexture`](bpy.types.VoronoiTexture.html#bpy.types.VoronoiTexture "bpy.types.VoronoiTexture"), [`WoodTexture`](bpy.types.WoodTexture.html#bpy.types.WoodTexture "bpy.types.WoodTexture")

_class _bpy.types.Texture(_ID_)
    

Texture data-block used by materials, lights, worlds and brushes

animation_data
    

Animation data for this data-block

Type:
    

[`AnimData`](bpy.types.AnimData.html#bpy.types.AnimData "bpy.types.AnimData"), (readonly)

color_ramp
    

Type:
    

[`ColorRamp`](bpy.types.ColorRamp.html#bpy.types.ColorRamp "bpy.types.ColorRamp"), (readonly)

contrast
    

Adjust the contrast of the texture

Type:
    

float in [0, 5], default 1.0

factor_blue
    

Type:
    

float in [0, 2], default 1.0

factor_green
    

Type:
    

float in [0, 2], default 1.0

factor_red
    

Type:
    

float in [0, 2], default 1.0

intensity
    

Adjust the brightness of the texture

Type:
    

float in [0, 2], default 1.0

node_tree
    

Node tree for node-based textures

Type:
    

[`NodeTree`](bpy.types.NodeTree.html#bpy.types.NodeTree "bpy.types.NodeTree"), (readonly)

saturation
    

Adjust the saturation of colors in the texture

Type:
    

float in [0, 2], default 1.0

type
    

Type:
    

enum in [Texture Type Items](bpy_types_enum_items/texture_type_items.html#rna-enum-texture-type-items), default `'IMAGE'`

use_clamp
    

Set negative texture RGB and intensity values to zero, for some uses like displacement this option can be disabled to get the full range

Type:
    

boolean, default False

use_color_ramp
    

Map the texture intensity to the color ramp. Note that the alpha value is used for image textures, enable “Calculate Alpha” for images without an alpha channel.

Type:
    

boolean, default False

use_nodes
    

Make this a node-based texture

Type:
    

boolean, default False

use_preview_alpha
    

Show Alpha in Preview Render

Type:
    

boolean, default False

users_material
    

Materials that use this texture

> type:
>     
> 
> tuple of [`Material`](bpy.types.Material.html#bpy.types.Material "bpy.types.Material")
> 
> Note
> 
> Takes `O(len(bpy.data.materials) * len(material.texture_slots))` time.

(readonly)

users_object_modifier
    

Object modifiers that use this texture

> type:
>     
> 
> tuple of [`Object`](bpy.types.Object.html#bpy.types.Object "bpy.types.Object")
> 
> Note
> 
> Takes `O(len(bpy.data.objects) * len(obj.modifiers))` time.

(readonly)

evaluate(_value_)
    

Evaluate the texture at the a given coordinate and returns the result

Parameters:
    

**value** ([`mathutils.Vector`](mathutils.html#mathutils.Vector "mathutils.Vector") of 3 items in [-inf, inf]) – The coordinates (x,y,z) of the texture, in case of a 3D texture, the z value is the slice of the texture that is evaluated. For 2D textures such as images, the z value is ignored.

Returns:
    

The result of the texture where (x,y,z,w) are (red, green, blue, intensity). For grayscale textures, often intensity only will be used.

Return type:
    

[`mathutils.Vector`](mathutils.html#mathutils.Vector "mathutils.Vector") of 4 items in [-inf, inf]

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

  * [`bpy.context.texture`](bpy.context.html#bpy.context.texture "bpy.context.texture")
  * [`BlendData.textures`](bpy.types.BlendData.html#bpy.types.BlendData.textures "bpy.types.BlendData.textures")
  * [`BlendDataTextures.new`](bpy.types.BlendDataTextures.html#bpy.types.BlendDataTextures.new "bpy.types.BlendDataTextures.new")
  * [`BlendDataTextures.remove`](bpy.types.BlendDataTextures.html#bpy.types.BlendDataTextures.remove "bpy.types.BlendDataTextures.remove")
  * [`Brush.mask_texture`](bpy.types.Brush.html#bpy.types.Brush.mask_texture "bpy.types.Brush.mask_texture")
  * [`Brush.texture`](bpy.types.Brush.html#bpy.types.Brush.texture "bpy.types.Brush.texture")
  * [`CompositorNodeTexture.texture`](bpy.types.CompositorNodeTexture.html#bpy.types.CompositorNodeTexture.texture "bpy.types.CompositorNodeTexture.texture")
  * [`DisplaceModifier.texture`](bpy.types.DisplaceModifier.html#bpy.types.DisplaceModifier.texture "bpy.types.DisplaceModifier.texture")
  * [`DynamicPaintSurface.init_texture`](bpy.types.DynamicPaintSurface.html#bpy.types.DynamicPaintSurface.init_texture "bpy.types.DynamicPaintSurface.init_texture")
  * [`FieldSettings.texture`](bpy.types.FieldSettings.html#bpy.types.FieldSettings.texture "bpy.types.FieldSettings.texture")
  * [`FluidFlowSettings.noise_texture`](bpy.types.FluidFlowSettings.html#bpy.types.FluidFlowSettings.noise_texture "bpy.types.FluidFlowSettings.noise_texture")
  * [`FreestyleLineStyle.active_texture`](bpy.types.FreestyleLineStyle.html#bpy.types.FreestyleLineStyle.active_texture "bpy.types.FreestyleLineStyle.active_texture")

| 

  * [`NodeSocketTexture.default_value`](bpy.types.NodeSocketTexture.html#bpy.types.NodeSocketTexture.default_value "bpy.types.NodeSocketTexture.default_value")
  * [`NodeTreeInterfaceSocketTexture.default_value`](bpy.types.NodeTreeInterfaceSocketTexture.html#bpy.types.NodeTreeInterfaceSocketTexture.default_value "bpy.types.NodeTreeInterfaceSocketTexture.default_value")
  * [`ParticleSettings.active_texture`](bpy.types.ParticleSettings.html#bpy.types.ParticleSettings.active_texture "bpy.types.ParticleSettings.active_texture")
  * [`TextureNodeTexture.texture`](bpy.types.TextureNodeTexture.html#bpy.types.TextureNodeTexture.texture "bpy.types.TextureNodeTexture.texture")
  * [`TextureSlot.texture`](bpy.types.TextureSlot.html#bpy.types.TextureSlot.texture "bpy.types.TextureSlot.texture")
  * [`VertexWeightEditModifier.mask_texture`](bpy.types.VertexWeightEditModifier.html#bpy.types.VertexWeightEditModifier.mask_texture "bpy.types.VertexWeightEditModifier.mask_texture")
  * [`VertexWeightMixModifier.mask_texture`](bpy.types.VertexWeightMixModifier.html#bpy.types.VertexWeightMixModifier.mask_texture "bpy.types.VertexWeightMixModifier.mask_texture")
  * [`VertexWeightProximityModifier.mask_texture`](bpy.types.VertexWeightProximityModifier.html#bpy.types.VertexWeightProximityModifier.mask_texture "bpy.types.VertexWeightProximityModifier.mask_texture")
  * [`VolumeDisplaceModifier.texture`](bpy.types.VolumeDisplaceModifier.html#bpy.types.VolumeDisplaceModifier.texture "bpy.types.VolumeDisplaceModifier.texture")
  * [`WarpModifier.texture`](bpy.types.WarpModifier.html#bpy.types.WarpModifier.texture "bpy.types.WarpModifier.texture")
  * [`WaveModifier.texture`](bpy.types.WaveModifier.html#bpy.types.WaveModifier.texture "bpy.types.WaveModifier.texture")

  
---|---
