# ShaderNode(NodeInternal)

base classes — [`bpy_struct`](bpy.types.bpy_struct.html#bpy.types.bpy_struct "bpy.types.bpy_struct"), [`Node`](bpy.types.Node.html#bpy.types.Node "bpy.types.Node"), [`NodeInternal`](bpy.types.NodeInternal.html#bpy.types.NodeInternal "bpy.types.NodeInternal")

subclasses — [`ShaderNodeAddShader`](bpy.types.ShaderNodeAddShader.html#bpy.types.ShaderNodeAddShader "bpy.types.ShaderNodeAddShader"), [`ShaderNodeAmbientOcclusion`](bpy.types.ShaderNodeAmbientOcclusion.html#bpy.types.ShaderNodeAmbientOcclusion "bpy.types.ShaderNodeAmbientOcclusion"), [`ShaderNodeAttribute`](bpy.types.ShaderNodeAttribute.html#bpy.types.ShaderNodeAttribute "bpy.types.ShaderNodeAttribute"), [`ShaderNodeBackground`](bpy.types.ShaderNodeBackground.html#bpy.types.ShaderNodeBackground "bpy.types.ShaderNodeBackground"), [`ShaderNodeBevel`](bpy.types.ShaderNodeBevel.html#bpy.types.ShaderNodeBevel "bpy.types.ShaderNodeBevel"), [`ShaderNodeBlackbody`](bpy.types.ShaderNodeBlackbody.html#bpy.types.ShaderNodeBlackbody "bpy.types.ShaderNodeBlackbody"), [`ShaderNodeBrightContrast`](bpy.types.ShaderNodeBrightContrast.html#bpy.types.ShaderNodeBrightContrast "bpy.types.ShaderNodeBrightContrast"), [`ShaderNodeBsdfAnisotropic`](bpy.types.ShaderNodeBsdfAnisotropic.html#bpy.types.ShaderNodeBsdfAnisotropic "bpy.types.ShaderNodeBsdfAnisotropic"), [`ShaderNodeBsdfDiffuse`](bpy.types.ShaderNodeBsdfDiffuse.html#bpy.types.ShaderNodeBsdfDiffuse "bpy.types.ShaderNodeBsdfDiffuse"), [`ShaderNodeBsdfGlass`](bpy.types.ShaderNodeBsdfGlass.html#bpy.types.ShaderNodeBsdfGlass "bpy.types.ShaderNodeBsdfGlass"), [`ShaderNodeBsdfHair`](bpy.types.ShaderNodeBsdfHair.html#bpy.types.ShaderNodeBsdfHair "bpy.types.ShaderNodeBsdfHair"), [`ShaderNodeBsdfHairPrincipled`](bpy.types.ShaderNodeBsdfHairPrincipled.html#bpy.types.ShaderNodeBsdfHairPrincipled "bpy.types.ShaderNodeBsdfHairPrincipled"), [`ShaderNodeBsdfMetallic`](bpy.types.ShaderNodeBsdfMetallic.html#bpy.types.ShaderNodeBsdfMetallic "bpy.types.ShaderNodeBsdfMetallic"), [`ShaderNodeBsdfPrincipled`](bpy.types.ShaderNodeBsdfPrincipled.html#bpy.types.ShaderNodeBsdfPrincipled "bpy.types.ShaderNodeBsdfPrincipled"), [`ShaderNodeBsdfRayPortal`](bpy.types.ShaderNodeBsdfRayPortal.html#bpy.types.ShaderNodeBsdfRayPortal "bpy.types.ShaderNodeBsdfRayPortal"), [`ShaderNodeBsdfRefraction`](bpy.types.ShaderNodeBsdfRefraction.html#bpy.types.ShaderNodeBsdfRefraction "bpy.types.ShaderNodeBsdfRefraction"), [`ShaderNodeBsdfSheen`](bpy.types.ShaderNodeBsdfSheen.html#bpy.types.ShaderNodeBsdfSheen "bpy.types.ShaderNodeBsdfSheen"), [`ShaderNodeBsdfToon`](bpy.types.ShaderNodeBsdfToon.html#bpy.types.ShaderNodeBsdfToon "bpy.types.ShaderNodeBsdfToon"), [`ShaderNodeBsdfTranslucent`](bpy.types.ShaderNodeBsdfTranslucent.html#bpy.types.ShaderNodeBsdfTranslucent "bpy.types.ShaderNodeBsdfTranslucent"), [`ShaderNodeBsdfTransparent`](bpy.types.ShaderNodeBsdfTransparent.html#bpy.types.ShaderNodeBsdfTransparent "bpy.types.ShaderNodeBsdfTransparent"), [`ShaderNodeBump`](bpy.types.ShaderNodeBump.html#bpy.types.ShaderNodeBump "bpy.types.ShaderNodeBump"), [`ShaderNodeCameraData`](bpy.types.ShaderNodeCameraData.html#bpy.types.ShaderNodeCameraData "bpy.types.ShaderNodeCameraData"), [`ShaderNodeClamp`](bpy.types.ShaderNodeClamp.html#bpy.types.ShaderNodeClamp "bpy.types.ShaderNodeClamp"), [`ShaderNodeCombineColor`](bpy.types.ShaderNodeCombineColor.html#bpy.types.ShaderNodeCombineColor "bpy.types.ShaderNodeCombineColor"), [`ShaderNodeCombineHSV`](bpy.types.ShaderNodeCombineHSV.html#bpy.types.ShaderNodeCombineHSV "bpy.types.ShaderNodeCombineHSV"), [`ShaderNodeCombineRGB`](bpy.types.ShaderNodeCombineRGB.html#bpy.types.ShaderNodeCombineRGB "bpy.types.ShaderNodeCombineRGB"), [`ShaderNodeCombineXYZ`](bpy.types.ShaderNodeCombineXYZ.html#bpy.types.ShaderNodeCombineXYZ "bpy.types.ShaderNodeCombineXYZ"), [`ShaderNodeCustomGroup`](bpy.types.ShaderNodeCustomGroup.html#bpy.types.ShaderNodeCustomGroup "bpy.types.ShaderNodeCustomGroup"), [`ShaderNodeDisplacement`](bpy.types.ShaderNodeDisplacement.html#bpy.types.ShaderNodeDisplacement "bpy.types.ShaderNodeDisplacement"), [`ShaderNodeEeveeSpecular`](bpy.types.ShaderNodeEeveeSpecular.html#bpy.types.ShaderNodeEeveeSpecular "bpy.types.ShaderNodeEeveeSpecular"), [`ShaderNodeEmission`](bpy.types.ShaderNodeEmission.html#bpy.types.ShaderNodeEmission "bpy.types.ShaderNodeEmission"), [`ShaderNodeFloatCurve`](bpy.types.ShaderNodeFloatCurve.html#bpy.types.ShaderNodeFloatCurve "bpy.types.ShaderNodeFloatCurve"), [`ShaderNodeFresnel`](bpy.types.ShaderNodeFresnel.html#bpy.types.ShaderNodeFresnel "bpy.types.ShaderNodeFresnel"), [`ShaderNodeGamma`](bpy.types.ShaderNodeGamma.html#bpy.types.ShaderNodeGamma "bpy.types.ShaderNodeGamma"), [`ShaderNodeGroup`](bpy.types.ShaderNodeGroup.html#bpy.types.ShaderNodeGroup "bpy.types.ShaderNodeGroup"), [`ShaderNodeHairInfo`](bpy.types.ShaderNodeHairInfo.html#bpy.types.ShaderNodeHairInfo "bpy.types.ShaderNodeHairInfo"), [`ShaderNodeHoldout`](bpy.types.ShaderNodeHoldout.html#bpy.types.ShaderNodeHoldout "bpy.types.ShaderNodeHoldout"), [`ShaderNodeHueSaturation`](bpy.types.ShaderNodeHueSaturation.html#bpy.types.ShaderNodeHueSaturation "bpy.types.ShaderNodeHueSaturation"), [`ShaderNodeInvert`](bpy.types.ShaderNodeInvert.html#bpy.types.ShaderNodeInvert "bpy.types.ShaderNodeInvert"), [`ShaderNodeLayerWeight`](bpy.types.ShaderNodeLayerWeight.html#bpy.types.ShaderNodeLayerWeight "bpy.types.ShaderNodeLayerWeight"), [`ShaderNodeLightFalloff`](bpy.types.ShaderNodeLightFalloff.html#bpy.types.ShaderNodeLightFalloff "bpy.types.ShaderNodeLightFalloff"), [`ShaderNodeLightPath`](bpy.types.ShaderNodeLightPath.html#bpy.types.ShaderNodeLightPath "bpy.types.ShaderNodeLightPath"), [`ShaderNodeMapRange`](bpy.types.ShaderNodeMapRange.html#bpy.types.ShaderNodeMapRange "bpy.types.ShaderNodeMapRange"), [`ShaderNodeMapping`](bpy.types.ShaderNodeMapping.html#bpy.types.ShaderNodeMapping "bpy.types.ShaderNodeMapping"), [`ShaderNodeMath`](bpy.types.ShaderNodeMath.html#bpy.types.ShaderNodeMath "bpy.types.ShaderNodeMath"), [`ShaderNodeMix`](bpy.types.ShaderNodeMix.html#bpy.types.ShaderNodeMix "bpy.types.ShaderNodeMix"), [`ShaderNodeMixRGB`](bpy.types.ShaderNodeMixRGB.html#bpy.types.ShaderNodeMixRGB "bpy.types.ShaderNodeMixRGB"), [`ShaderNodeMixShader`](bpy.types.ShaderNodeMixShader.html#bpy.types.ShaderNodeMixShader "bpy.types.ShaderNodeMixShader"), [`ShaderNodeNewGeometry`](bpy.types.ShaderNodeNewGeometry.html#bpy.types.ShaderNodeNewGeometry "bpy.types.ShaderNodeNewGeometry"), [`ShaderNodeNormal`](bpy.types.ShaderNodeNormal.html#bpy.types.ShaderNodeNormal "bpy.types.ShaderNodeNormal"), [`ShaderNodeNormalMap`](bpy.types.ShaderNodeNormalMap.html#bpy.types.ShaderNodeNormalMap "bpy.types.ShaderNodeNormalMap"), [`ShaderNodeObjectInfo`](bpy.types.ShaderNodeObjectInfo.html#bpy.types.ShaderNodeObjectInfo "bpy.types.ShaderNodeObjectInfo"), [`ShaderNodeOutputAOV`](bpy.types.ShaderNodeOutputAOV.html#bpy.types.ShaderNodeOutputAOV "bpy.types.ShaderNodeOutputAOV"), [`ShaderNodeOutputLight`](bpy.types.ShaderNodeOutputLight.html#bpy.types.ShaderNodeOutputLight "bpy.types.ShaderNodeOutputLight"), [`ShaderNodeOutputLineStyle`](bpy.types.ShaderNodeOutputLineStyle.html#bpy.types.ShaderNodeOutputLineStyle "bpy.types.ShaderNodeOutputLineStyle"), [`ShaderNodeOutputMaterial`](bpy.types.ShaderNodeOutputMaterial.html#bpy.types.ShaderNodeOutputMaterial "bpy.types.ShaderNodeOutputMaterial"), [`ShaderNodeOutputWorld`](bpy.types.ShaderNodeOutputWorld.html#bpy.types.ShaderNodeOutputWorld "bpy.types.ShaderNodeOutputWorld"), [`ShaderNodeParticleInfo`](bpy.types.ShaderNodeParticleInfo.html#bpy.types.ShaderNodeParticleInfo "bpy.types.ShaderNodeParticleInfo"), [`ShaderNodePointInfo`](bpy.types.ShaderNodePointInfo.html#bpy.types.ShaderNodePointInfo "bpy.types.ShaderNodePointInfo"), [`ShaderNodeRGB`](bpy.types.ShaderNodeRGB.html#bpy.types.ShaderNodeRGB "bpy.types.ShaderNodeRGB"), [`ShaderNodeRGBCurve`](bpy.types.ShaderNodeRGBCurve.html#bpy.types.ShaderNodeRGBCurve "bpy.types.ShaderNodeRGBCurve"), [`ShaderNodeRGBToBW`](bpy.types.ShaderNodeRGBToBW.html#bpy.types.ShaderNodeRGBToBW "bpy.types.ShaderNodeRGBToBW"), [`ShaderNodeScript`](bpy.types.ShaderNodeScript.html#bpy.types.ShaderNodeScript "bpy.types.ShaderNodeScript"), [`ShaderNodeSeparateColor`](bpy.types.ShaderNodeSeparateColor.html#bpy.types.ShaderNodeSeparateColor "bpy.types.ShaderNodeSeparateColor"), [`ShaderNodeSeparateHSV`](bpy.types.ShaderNodeSeparateHSV.html#bpy.types.ShaderNodeSeparateHSV "bpy.types.ShaderNodeSeparateHSV"), [`ShaderNodeSeparateRGB`](bpy.types.ShaderNodeSeparateRGB.html#bpy.types.ShaderNodeSeparateRGB "bpy.types.ShaderNodeSeparateRGB"), [`ShaderNodeSeparateXYZ`](bpy.types.ShaderNodeSeparateXYZ.html#bpy.types.ShaderNodeSeparateXYZ "bpy.types.ShaderNodeSeparateXYZ"), [`ShaderNodeShaderToRGB`](bpy.types.ShaderNodeShaderToRGB.html#bpy.types.ShaderNodeShaderToRGB "bpy.types.ShaderNodeShaderToRGB"), [`ShaderNodeSqueeze`](bpy.types.ShaderNodeSqueeze.html#bpy.types.ShaderNodeSqueeze "bpy.types.ShaderNodeSqueeze"), [`ShaderNodeSubsurfaceScattering`](bpy.types.ShaderNodeSubsurfaceScattering.html#bpy.types.ShaderNodeSubsurfaceScattering "bpy.types.ShaderNodeSubsurfaceScattering"), [`ShaderNodeTangent`](bpy.types.ShaderNodeTangent.html#bpy.types.ShaderNodeTangent "bpy.types.ShaderNodeTangent"), [`ShaderNodeTexBrick`](bpy.types.ShaderNodeTexBrick.html#bpy.types.ShaderNodeTexBrick "bpy.types.ShaderNodeTexBrick"), [`ShaderNodeTexChecker`](bpy.types.ShaderNodeTexChecker.html#bpy.types.ShaderNodeTexChecker "bpy.types.ShaderNodeTexChecker"), [`ShaderNodeTexCoord`](bpy.types.ShaderNodeTexCoord.html#bpy.types.ShaderNodeTexCoord "bpy.types.ShaderNodeTexCoord"), [`ShaderNodeTexEnvironment`](bpy.types.ShaderNodeTexEnvironment.html#bpy.types.ShaderNodeTexEnvironment "bpy.types.ShaderNodeTexEnvironment"), [`ShaderNodeTexGabor`](bpy.types.ShaderNodeTexGabor.html#bpy.types.ShaderNodeTexGabor "bpy.types.ShaderNodeTexGabor"), [`ShaderNodeTexGradient`](bpy.types.ShaderNodeTexGradient.html#bpy.types.ShaderNodeTexGradient "bpy.types.ShaderNodeTexGradient"), [`ShaderNodeTexIES`](bpy.types.ShaderNodeTexIES.html#bpy.types.ShaderNodeTexIES "bpy.types.ShaderNodeTexIES"), [`ShaderNodeTexImage`](bpy.types.ShaderNodeTexImage.html#bpy.types.ShaderNodeTexImage "bpy.types.ShaderNodeTexImage"), [`ShaderNodeTexMagic`](bpy.types.ShaderNodeTexMagic.html#bpy.types.ShaderNodeTexMagic "bpy.types.ShaderNodeTexMagic"), [`ShaderNodeTexNoise`](bpy.types.ShaderNodeTexNoise.html#bpy.types.ShaderNodeTexNoise "bpy.types.ShaderNodeTexNoise"), [`ShaderNodeTexPointDensity`](bpy.types.ShaderNodeTexPointDensity.html#bpy.types.ShaderNodeTexPointDensity "bpy.types.ShaderNodeTexPointDensity"), [`ShaderNodeTexSky`](bpy.types.ShaderNodeTexSky.html#bpy.types.ShaderNodeTexSky "bpy.types.ShaderNodeTexSky"), [`ShaderNodeTexVoronoi`](bpy.types.ShaderNodeTexVoronoi.html#bpy.types.ShaderNodeTexVoronoi "bpy.types.ShaderNodeTexVoronoi"), [`ShaderNodeTexWave`](bpy.types.ShaderNodeTexWave.html#bpy.types.ShaderNodeTexWave "bpy.types.ShaderNodeTexWave"), [`ShaderNodeTexWhiteNoise`](bpy.types.ShaderNodeTexWhiteNoise.html#bpy.types.ShaderNodeTexWhiteNoise "bpy.types.ShaderNodeTexWhiteNoise"), [`ShaderNodeUVAlongStroke`](bpy.types.ShaderNodeUVAlongStroke.html#bpy.types.ShaderNodeUVAlongStroke "bpy.types.ShaderNodeUVAlongStroke"), [`ShaderNodeUVMap`](bpy.types.ShaderNodeUVMap.html#bpy.types.ShaderNodeUVMap "bpy.types.ShaderNodeUVMap"), [`ShaderNodeValToRGB`](bpy.types.ShaderNodeValToRGB.html#bpy.types.ShaderNodeValToRGB "bpy.types.ShaderNodeValToRGB"), [`ShaderNodeValue`](bpy.types.ShaderNodeValue.html#bpy.types.ShaderNodeValue "bpy.types.ShaderNodeValue"), [`ShaderNodeVectorCurve`](bpy.types.ShaderNodeVectorCurve.html#bpy.types.ShaderNodeVectorCurve "bpy.types.ShaderNodeVectorCurve"), [`ShaderNodeVectorDisplacement`](bpy.types.ShaderNodeVectorDisplacement.html#bpy.types.ShaderNodeVectorDisplacement "bpy.types.ShaderNodeVectorDisplacement"), [`ShaderNodeVectorMath`](bpy.types.ShaderNodeVectorMath.html#bpy.types.ShaderNodeVectorMath "bpy.types.ShaderNodeVectorMath"), [`ShaderNodeVectorRotate`](bpy.types.ShaderNodeVectorRotate.html#bpy.types.ShaderNodeVectorRotate "bpy.types.ShaderNodeVectorRotate"), [`ShaderNodeVectorTransform`](bpy.types.ShaderNodeVectorTransform.html#bpy.types.ShaderNodeVectorTransform "bpy.types.ShaderNodeVectorTransform"), [`ShaderNodeVertexColor`](bpy.types.ShaderNodeVertexColor.html#bpy.types.ShaderNodeVertexColor "bpy.types.ShaderNodeVertexColor"), [`ShaderNodeVolumeAbsorption`](bpy.types.ShaderNodeVolumeAbsorption.html#bpy.types.ShaderNodeVolumeAbsorption "bpy.types.ShaderNodeVolumeAbsorption"), [`ShaderNodeVolumeCoefficients`](bpy.types.ShaderNodeVolumeCoefficients.html#bpy.types.ShaderNodeVolumeCoefficients "bpy.types.ShaderNodeVolumeCoefficients"), [`ShaderNodeVolumeInfo`](bpy.types.ShaderNodeVolumeInfo.html#bpy.types.ShaderNodeVolumeInfo "bpy.types.ShaderNodeVolumeInfo"), [`ShaderNodeVolumePrincipled`](bpy.types.ShaderNodeVolumePrincipled.html#bpy.types.ShaderNodeVolumePrincipled "bpy.types.ShaderNodeVolumePrincipled"), [`ShaderNodeVolumeScatter`](bpy.types.ShaderNodeVolumeScatter.html#bpy.types.ShaderNodeVolumeScatter "bpy.types.ShaderNodeVolumeScatter"), [`ShaderNodeWavelength`](bpy.types.ShaderNodeWavelength.html#bpy.types.ShaderNodeWavelength "bpy.types.ShaderNodeWavelength"), [`ShaderNodeWireframe`](bpy.types.ShaderNodeWireframe.html#bpy.types.ShaderNodeWireframe "bpy.types.ShaderNodeWireframe")

_class _bpy.types.ShaderNode(_NodeInternal_)
    

Material shader node

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
  * [`Node.type`](bpy.types.Node.html#bpy.types.Node.type "bpy.types.Node.type")
  * [`Node.location`](bpy.types.Node.html#bpy.types.Node.location "bpy.types.Node.location")
  * [`Node.location_absolute`](bpy.types.Node.html#bpy.types.Node.location_absolute "bpy.types.Node.location_absolute")
  * [`Node.width`](bpy.types.Node.html#bpy.types.Node.width "bpy.types.Node.width")
  * [`Node.height`](bpy.types.Node.html#bpy.types.Node.height "bpy.types.Node.height")
  * [`Node.dimensions`](bpy.types.Node.html#bpy.types.Node.dimensions "bpy.types.Node.dimensions")
  * [`Node.name`](bpy.types.Node.html#bpy.types.Node.name "bpy.types.Node.name")
  * [`Node.label`](bpy.types.Node.html#bpy.types.Node.label "bpy.types.Node.label")
  * [`Node.inputs`](bpy.types.Node.html#bpy.types.Node.inputs "bpy.types.Node.inputs")
  * [`Node.outputs`](bpy.types.Node.html#bpy.types.Node.outputs "bpy.types.Node.outputs")
  * [`Node.internal_links`](bpy.types.Node.html#bpy.types.Node.internal_links "bpy.types.Node.internal_links")
  * [`Node.parent`](bpy.types.Node.html#bpy.types.Node.parent "bpy.types.Node.parent")
  * [`Node.warning_propagation`](bpy.types.Node.html#bpy.types.Node.warning_propagation "bpy.types.Node.warning_propagation")
  * [`Node.use_custom_color`](bpy.types.Node.html#bpy.types.Node.use_custom_color "bpy.types.Node.use_custom_color")
  * [`Node.color`](bpy.types.Node.html#bpy.types.Node.color "bpy.types.Node.color")
  * [`Node.color_tag`](bpy.types.Node.html#bpy.types.Node.color_tag "bpy.types.Node.color_tag")

| 

  * [`Node.select`](bpy.types.Node.html#bpy.types.Node.select "bpy.types.Node.select")
  * [`Node.show_options`](bpy.types.Node.html#bpy.types.Node.show_options "bpy.types.Node.show_options")
  * [`Node.show_preview`](bpy.types.Node.html#bpy.types.Node.show_preview "bpy.types.Node.show_preview")
  * [`Node.hide`](bpy.types.Node.html#bpy.types.Node.hide "bpy.types.Node.hide")
  * [`Node.mute`](bpy.types.Node.html#bpy.types.Node.mute "bpy.types.Node.mute")
  * [`Node.show_texture`](bpy.types.Node.html#bpy.types.Node.show_texture "bpy.types.Node.show_texture")
  * [`Node.bl_idname`](bpy.types.Node.html#bpy.types.Node.bl_idname "bpy.types.Node.bl_idname")
  * [`Node.bl_label`](bpy.types.Node.html#bpy.types.Node.bl_label "bpy.types.Node.bl_label")
  * [`Node.bl_description`](bpy.types.Node.html#bpy.types.Node.bl_description "bpy.types.Node.bl_description")
  * [`Node.bl_icon`](bpy.types.Node.html#bpy.types.Node.bl_icon "bpy.types.Node.bl_icon")
  * [`Node.bl_static_type`](bpy.types.Node.html#bpy.types.Node.bl_static_type "bpy.types.Node.bl_static_type")
  * [`Node.bl_width_default`](bpy.types.Node.html#bpy.types.Node.bl_width_default "bpy.types.Node.bl_width_default")
  * [`Node.bl_width_min`](bpy.types.Node.html#bpy.types.Node.bl_width_min "bpy.types.Node.bl_width_min")
  * [`Node.bl_width_max`](bpy.types.Node.html#bpy.types.Node.bl_width_max "bpy.types.Node.bl_width_max")
  * [`Node.bl_height_default`](bpy.types.Node.html#bpy.types.Node.bl_height_default "bpy.types.Node.bl_height_default")
  * [`Node.bl_height_min`](bpy.types.Node.html#bpy.types.Node.bl_height_min "bpy.types.Node.bl_height_min")
  * [`Node.bl_height_max`](bpy.types.Node.html#bpy.types.Node.bl_height_max "bpy.types.Node.bl_height_max")

  
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
  * [`bpy_struct.type_recast`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.type_recast "bpy.types.bpy_struct.type_recast")
  * [`bpy_struct.values`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.values "bpy.types.bpy_struct.values")
  * [`Node.socket_value_update`](bpy.types.Node.html#bpy.types.Node.socket_value_update "bpy.types.Node.socket_value_update")

| 

  * [`Node.is_registered_node_type`](bpy.types.Node.html#bpy.types.Node.is_registered_node_type "bpy.types.Node.is_registered_node_type")
  * [`Node.poll`](bpy.types.Node.html#bpy.types.Node.poll "bpy.types.Node.poll")
  * [`Node.poll_instance`](bpy.types.Node.html#bpy.types.Node.poll_instance "bpy.types.Node.poll_instance")
  * [`Node.update`](bpy.types.Node.html#bpy.types.Node.update "bpy.types.Node.update")
  * [`Node.insert_link`](bpy.types.Node.html#bpy.types.Node.insert_link "bpy.types.Node.insert_link")
  * [`Node.init`](bpy.types.Node.html#bpy.types.Node.init "bpy.types.Node.init")
  * [`Node.copy`](bpy.types.Node.html#bpy.types.Node.copy "bpy.types.Node.copy")
  * [`Node.free`](bpy.types.Node.html#bpy.types.Node.free "bpy.types.Node.free")
  * [`Node.draw_buttons`](bpy.types.Node.html#bpy.types.Node.draw_buttons "bpy.types.Node.draw_buttons")
  * [`Node.draw_buttons_ext`](bpy.types.Node.html#bpy.types.Node.draw_buttons_ext "bpy.types.Node.draw_buttons_ext")
  * [`Node.draw_label`](bpy.types.Node.html#bpy.types.Node.draw_label "bpy.types.Node.draw_label")
  * [`Node.debug_zone_body_lazy_function_graph`](bpy.types.Node.html#bpy.types.Node.debug_zone_body_lazy_function_graph "bpy.types.Node.debug_zone_body_lazy_function_graph")
  * [`Node.debug_zone_lazy_function_graph`](bpy.types.Node.html#bpy.types.Node.debug_zone_lazy_function_graph "bpy.types.Node.debug_zone_lazy_function_graph")
  * [`Node.poll`](bpy.types.Node.html#bpy.types.Node.poll "bpy.types.Node.poll")
  * [`Node.bl_rna_get_subclass`](bpy.types.Node.html#bpy.types.Node.bl_rna_get_subclass "bpy.types.Node.bl_rna_get_subclass")
  * [`Node.bl_rna_get_subclass_py`](bpy.types.Node.html#bpy.types.Node.bl_rna_get_subclass_py "bpy.types.Node.bl_rna_get_subclass_py")
  * [`NodeInternal.poll`](bpy.types.NodeInternal.html#bpy.types.NodeInternal.poll "bpy.types.NodeInternal.poll")
  * [`NodeInternal.poll_instance`](bpy.types.NodeInternal.html#bpy.types.NodeInternal.poll_instance "bpy.types.NodeInternal.poll_instance")
  * [`NodeInternal.update`](bpy.types.NodeInternal.html#bpy.types.NodeInternal.update "bpy.types.NodeInternal.update")
  * [`NodeInternal.draw_buttons`](bpy.types.NodeInternal.html#bpy.types.NodeInternal.draw_buttons "bpy.types.NodeInternal.draw_buttons")
  * [`NodeInternal.draw_buttons_ext`](bpy.types.NodeInternal.html#bpy.types.NodeInternal.draw_buttons_ext "bpy.types.NodeInternal.draw_buttons_ext")
  * [`NodeInternal.bl_rna_get_subclass`](bpy.types.NodeInternal.html#bpy.types.NodeInternal.bl_rna_get_subclass "bpy.types.NodeInternal.bl_rna_get_subclass")
  * [`NodeInternal.bl_rna_get_subclass_py`](bpy.types.NodeInternal.html#bpy.types.NodeInternal.bl_rna_get_subclass_py "bpy.types.NodeInternal.bl_rna_get_subclass_py")

  
---|---  
  
## References

  * [`ShaderNodeTree.get_output_node`](bpy.types.ShaderNodeTree.html#bpy.types.ShaderNodeTree.get_output_node "bpy.types.ShaderNodeTree.get_output_node")

| 


  
---|---
