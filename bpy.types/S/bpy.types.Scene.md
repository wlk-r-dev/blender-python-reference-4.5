# Scene(ID)

base classes — [[bpy_struct]], [[ID]]

_class _bpy.types.Scene(_ID_)
    

Scene data-block, consisting in objects and defining time and render related settings

active_clip
    

Active Movie Clip that can be used by motion tracking constraints or as a camera’s background image

Type:
    

[[MovieClip]]

animation_data
    

Animation data for this data-block

Type:
    

[[AnimData]], (readonly)

audio_distance_model
    

Distance model for distance attenuation calculation

  * `NONE` None – No distance attenuation.

  * `INVERSE` Inverse – Inverse distance model.

  * `INVERSE_CLAMPED` Inverse Clamped – Inverse distance model with clamping.

  * `LINEAR` Linear – Linear distance model.

  * `LINEAR_CLAMPED` Linear Clamped – Linear distance model with clamping.

  * `EXPONENT` Exponential – Exponential distance model.

  * `EXPONENT_CLAMPED` Exponential Clamped – Exponential distance model with clamping.


Type:
    

enum in [`'NONE'`, `'INVERSE'`, `'INVERSE_CLAMPED'`, `'LINEAR'`, `'LINEAR_CLAMPED'`, `'EXPONENT'`, `'EXPONENT_CLAMPED'`], default `'NONE'`

audio_doppler_factor
    

Pitch factor for Doppler effect calculation

Type:
    

float in [0, inf], default 1.0

audio_doppler_speed
    

Speed of sound for Doppler effect calculation

Type:
    

float in [0.01, inf], default 343.3

audio_volume
    

Audio volume

Type:
    

float in [0, 100], default 1.0

background_set
    

Background set scene

Type:
    

`Scene`

camera
    

Active camera, used for rendering the scene

Type:
    

[[Object]]

collection
    

Scene root collection that owns all the objects and other collections instantiated in the scene

Type:
    

[[Collection]], (readonly, never None)

cursor
    

Type:
    

[[View3DCursor]], (readonly, never None)

cycles
    

Cycles render settings

Type:
    

`CyclesRenderSettings`, (readonly)

cycles_curves
    

Cycles curves rendering settings

Type:
    

`CyclesCurveRenderSettings`, (readonly)

display
    

Scene display settings for 3D viewport

Type:
    

[[SceneDisplay]], (readonly)

display_settings
    

Settings of device saved image would be displayed on

Type:
    

[[ColorManagedDisplaySettings]], (readonly)

eevee
    

EEVEE settings for the scene

Type:
    

[[SceneEEVEE]], (readonly)

frame_current
    

Current frame, to update animation data from Python frame_set() instead

Type:
    

int in [-1048574, 1048574], default 1

frame_current_final
    

Current frame with subframe and time remapping applied

Type:
    

float in [-1.04857e+06, 1.04857e+06], default 0.0, (readonly)

frame_end
    

Final frame of the playback/rendering range

Type:
    

int in [0, 1048574], default 250

frame_float
    

Type:
    

float in [-1.04857e+06, 1.04857e+06], default 0.0

frame_preview_end
    

Alternative end frame for UI playback

Type:
    

int in [-inf, inf], default 0

frame_preview_start
    

Alternative start frame for UI playback

Type:
    

int in [-inf, inf], default 0

frame_start
    

First frame of the playback/rendering range

Type:
    

int in [0, 1048574], default 1

frame_step
    

Number of frames to skip forward while rendering/playing back each frame

Type:
    

int in [0, 1048574], default 1

frame_subframe
    

Type:
    

float in [0, 1], default 0.0

gravity
    

Constant acceleration in a given direction

Type:
    

[[mathutils.Vector]] of 3 items in [-inf, inf], default (0.0, 0.0, -9.81)

grease_pencil
    

Grease Pencil data-block used for annotations in the 3D view

Type:
    

[[GreasePencil]]

grease_pencil_settings
    

Grease Pencil settings for the scene

Type:
    

[[SceneGpencil]], (readonly)

hydra
    

Hydra settings for the scene

Type:
    

[[SceneHydra]], (readonly)

is_nla_tweakmode
    

Whether there is any action referenced by NLA being edited (strictly read-only)

Type:
    

boolean, default False, (readonly)

keying_sets
    

Absolute Keying Sets for this Scene

Type:
    

[[KeyingSets]] [[bpy_prop_collection]] of [[KeyingSet]], (readonly)

keying_sets_all
    

All Keying Sets available for use (Builtins and Absolute Keying Sets for this Scene)

Type:
    

[[KeyingSetsAll]] [[bpy_prop_collection]] of [[KeyingSet]], (readonly)

lock_frame_selection_to_range
    

Don’t allow frame to be selected with mouse outside of frame range

Type:
    

boolean, default False

node_tree
    

Compositing node tree

Type:
    

[[NodeTree]], (readonly)

objects
    

Type:
    

[[SceneObjects]] [[bpy_prop_collection]] of [[Object]], (readonly)

render
    

Type:
    

[[RenderSettings]], (readonly, never None)

rigidbody_world
    

Type:
    

[[RigidBodyWorld]], (readonly)

safe_areas
    

Type:
    

[[DisplaySafeAreas]], (readonly, never None)

sequence_editor
    

Type:
    

[[SequenceEditor]], (readonly)

sequencer_colorspace_settings
    

Settings of color space sequencer is working in

Type:
    

[[ColorManagedSequencerColorspaceSettings]], (readonly)

show_keys_from_selected_only
    

Only include channels relating to selected objects and data

Type:
    

boolean, default True

show_subframe
    

Display and allow setting fractional frame values for the current frame

Type:
    

boolean, default False

simulation_frame_end
    

Frame at which simulations end

Type:
    

int in [-inf, inf], default 250

simulation_frame_start
    

Frame at which simulations start

Type:
    

int in [-inf, inf], default 1

sync_mode
    

How to sync playback

  * `NONE` Play Every Frame – Do not sync, play every frame.

  * `FRAME_DROP` Frame Dropping – Drop frames if playback is too slow.

  * `AUDIO_SYNC` Sync to Audio – Sync to audio playback, dropping frames.


Type:
    

enum in [`'NONE'`, `'FRAME_DROP'`, `'AUDIO_SYNC'`], default `'AUDIO_SYNC'`

timeline_markers
    

Markers used in all timelines for the current scene

Type:
    

[[TimelineMarkers]] [[bpy_prop_collection]] of [[TimelineMarker]], (readonly)

tool_settings
    

Type:
    

[[ToolSettings]], (readonly, never None)

transform_orientation_slots
    

Type:
    

[[bpy_prop_collection]] of [[TransformOrientationSlot]], (readonly)

unit_settings
    

Unit editing settings

Type:
    

[[UnitSettings]], (readonly, never None)

use_audio
    

Play back of audio from Sequence Editor, otherwise mute audio

Type:
    

boolean, default False

use_audio_scrub
    

Play audio from Sequence Editor while scrubbing

Type:
    

boolean, default False

use_custom_simulation_range
    

Use a simulation range that is different from the scene range for simulation nodes that don’t override the frame range themselves

Type:
    

boolean, default False

use_gravity
    

Use global gravity for all dynamics

Type:
    

boolean, default True

use_nodes
    

Enable the compositing node tree

Type:
    

boolean, default False

use_preview_range
    

Use an alternative start/end frame range for animation playback and view renders

Type:
    

boolean, default False

use_stamp_note
    

User defined note for the render stamping

Type:
    

string, default “”, (never None)

view_layers
    

Type:
    

[[ViewLayers]] [[bpy_prop_collection]] of [[ViewLayer]], (readonly)

view_settings
    

Color management settings applied on image before saving

Type:
    

[[ColorManagedViewSettings]], (readonly)

world
    

World used for rendering the scene

Type:
    

[[World]]

_classmethod _update_render_engine()
    

Trigger a render engine update

statistics(_view_layer_)
    

statistics

Parameters:
    

**view_layer** ([[ViewLayer]], (never None)) – View Layer

Returns:
    

Statistics

Return type:
    

string, (never None)

frame_set(_frame_ , _*_ , _subframe =0.0_)
    

Set scene frame updating all objects and view layers immediately

Parameters:
    

  * **frame** (_int in_ _[__-1048574_ _,__1048574_ _]_) – Frame number to set

  * **subframe** (_float in_ _[__0_ _,__1_ _]__,__(__optional_ _)_) – Subframe time, between 0.0 and 1.0


uvedit_aspect(_object_)
    

Get uv aspect for current object

Parameters:
    

**object** ([[Object]], (never None)) – Object

Returns:
    

aspect

Return type:
    

[[mathutils.Vector]] of 2 items in [0, inf]

ray_cast(_depsgraph_ , _origin_ , _direction_ , _*_ , _distance =1.70141e+38_)
    

Cast a ray onto evaluated geometry in world-space

Parameters:
    

  * **depsgraph** ([[Depsgraph]], (never None)) – The current dependency graph

  * **distance** (_float in_ _[__0_ _,__inf_ _]__,__(__optional_ _)_) – Maximum distance


Returns:
    

result, boolean

location, The hit location of this ray cast, [[mathutils.Vector]] of 3 items in [-inf, inf]

normal, The face normal at the ray cast hit location, [[mathutils.Vector]] of 3 items in [-inf, inf]

index, The face index, -1 when original data isn’t available, int in [-inf, inf]

object, Ray cast object, [[Object]]

matrix, Matrix, [[mathutils.Matrix]] of 4 * 4 items in [-inf, inf]

Return type:
    

(boolean, [[mathutils.Vector]] of 3 items in [-inf, inf], [[mathutils.Vector]] of 3 items in [-inf, inf], int in [-inf, inf], [[Object]], [[mathutils.Matrix]] of 4 * 4 items in [-inf, inf])

sequence_editor_create()
    

Ensure sequence editor is valid in this scene

Returns:
    

New sequence editor data or nullptr

Return type:
    

[[SequenceEditor]]

sequence_editor_clear()
    

Clear sequence editor in this scene

alembic_export(_filepath_ , _*_ , _frame_start =1_, _frame_end =1_, _xform_samples =1_, _geom_samples =1_, _shutter_open =0.0_, _shutter_close =1.0_, _selected_only =False_, _uvs =True_, _normals =True_, _vcolors =False_, _apply_subdiv =True_, _flatten =False_, _visible_objects_only =False_, _face_sets =False_, _subdiv_schema =False_, _export_hair =True_, _export_particles =True_, _packuv =False_, _scale =1.0_, _triangulate =False_, _quad_method ='BEAUTY'_, _ngon_method ='BEAUTY'_)
    

Export to Alembic file (deprecated, use the Alembic export operator)

Parameters:
    

  * **filepath** (_string_ _,__(__never None_ _)_) – File Path, File path to write Alembic file

  * **frame_start** (_int in_ _[__-inf_ _,__inf_ _]__,__(__optional_ _)_) – Start, Start Frame

  * **frame_end** (_int in_ _[__-inf_ _,__inf_ _]__,__(__optional_ _)_) – End, End Frame

  * **xform_samples** (_int in_ _[__1_ _,__128_ _]__,__(__optional_ _)_) – Xform samples, Transform samples per frame

  * **geom_samples** (_int in_ _[__1_ _,__128_ _]__,__(__optional_ _)_) – Geom samples, Geometry samples per frame

  * **shutter_open** (_float in_ _[__-1_ _,__1_ _]__,__(__optional_ _)_) – Shutter open

  * **shutter_close** (_float in_ _[__-1_ _,__1_ _]__,__(__optional_ _)_) – Shutter close

  * **selected_only** (_boolean_ _,__(__optional_ _)_) – Selected only, Export only selected objects

  * **uvs** (_boolean_ _,__(__optional_ _)_) – UVs, Export UVs

  * **normals** (_boolean_ _,__(__optional_ _)_) – Normals, Export normals

  * **vcolors** (_boolean_ _,__(__optional_ _)_) – Color Attributes, Export color attributes

  * **apply_subdiv** (_boolean_ _,__(__optional_ _)_) – Subsurfs as meshes, Export subdivision surfaces as meshes

  * **flatten** (_boolean_ _,__(__optional_ _)_) – Flatten hierarchy, Flatten hierarchy

  * **visible_objects_only** (_boolean_ _,__(__optional_ _)_) – Visible layers only, Export only objects in visible layers

  * **face_sets** (_boolean_ _,__(__optional_ _)_) – Facesets, Export face sets

  * **subdiv_schema** (_boolean_ _,__(__optional_ _)_) – Use Alembic subdivision Schema, Use Alembic subdivision Schema

  * **export_hair** (_boolean_ _,__(__optional_ _)_) – Export Hair, Exports hair particle systems as animated curves

  * **export_particles** (_boolean_ _,__(__optional_ _)_) – Export Particles, Exports non-hair particle systems

  * **packuv** (_boolean_ _,__(__optional_ _)_) – Export with packed UV islands, Export with packed UV islands

  * **scale** (_float in_ _[__0.0001_ _,__1000_ _]__,__(__optional_ _)_) – Scale, Value by which to enlarge or shrink the objects with respect to the world’s origin

  * **triangulate** (_boolean_ _,__(__optional_ _)_) – Triangulate, Export polygons (quads and n-gons) as triangles

  * **quad_method** (enum in [Modifier Triangulate Quad Method Items](bpy_types_enum_items/modifier_triangulate_quad_method_items.md#rna-enum-modifier-triangulate-quad-method-items), (optional)) – Quad Method, Method for splitting the quads into triangles

  * **ngon_method** (enum in [Modifier Triangulate Ngon Method Items](bpy_types_enum_items/modifier_triangulate_ngon_method_items.md#rna-enum-modifier-triangulate-ngon-method-items), (optional)) – N-gon Method, Method for splitting the n-gons into triangles


_classmethod _bl_rna_get_subclass(_id_ , _default =None_, _/_)
    

Parameters:
    

**id** (_str_) – The RNA type identifier.

Returns:
    

The RNA type or default when not found.

Return type:
    

[[bpy.types.Struct]] subclass

_classmethod _bl_rna_get_subclass_py(_id_ , _default =None_, _/_)
    

Parameters:
    

**id** (_str_) – The RNA type identifier.

Returns:
    

The class or default when not found.

Return type:
    

type

## Inherited Properties

  * [[bpy_struct.id_data]]
  * [[ID.name]]
  * [[ID.name_full]]
  * [[ID.id_type]]
  * [[ID.session_uid]]
  * [[ID.is_evaluated]]
  * [[ID.original]]
  * [[ID.users]]
  * [[ID.use_fake_user]]
  * [[ID.use_extra_user]]
  * [[ID.is_embedded_data]]

| 

  * [[ID.is_missing]]
  * [[ID.is_runtime_data]]
  * [[ID.is_editable]]
  * [[ID.tag]]
  * [[ID.is_library_indirect]]
  * [[ID.library]]
  * [[ID.library_weak_reference]]
  * [[ID.asset_data]]
  * [[ID.override_library]]
  * [[ID.preview]]

  
---|---  
  
## Inherited Functions

  * [[bpy_struct.as_pointer]]
  * [[bpy_struct.driver_add]]
  * [[bpy_struct.driver_remove]]
  * [[bpy_struct.get]]
  * [[bpy_struct.id_properties_clear]]
  * [[bpy_struct.id_properties_ensure]]
  * [[bpy_struct.id_properties_ui]]
  * [[bpy_struct.is_property_hidden]]
  * [[bpy_struct.is_property_overridable_library]]
  * [[bpy_struct.is_property_readonly]]
  * [[bpy_struct.is_property_set]]
  * [[bpy_struct.items]]
  * [[bpy_struct.keyframe_delete]]
  * [[bpy_struct.keyframe_insert]]
  * [[bpy_struct.keys]]
  * [[bpy_struct.path_from_id]]
  * [[bpy_struct.path_resolve]]
  * [[bpy_struct.pop]]
  * [[bpy_struct.property_overridable_library_set]]
  * [[bpy_struct.property_unset]]
  * [[bpy_struct.rna_ancestors]]

| 

  * [[bpy_struct.type_recast]]
  * [[bpy_struct.values]]
  * [[ID.rename]]
  * [[ID.evaluated_get]]
  * [[ID.copy]]
  * [[ID.asset_mark]]
  * [[ID.asset_clear]]
  * [[ID.asset_generate_preview]]
  * [[ID.override_create]]
  * [[ID.override_hierarchy_create]]
  * [[ID.user_clear]]
  * [[ID.user_remap]]
  * [[ID.make_local]]
  * [[ID.user_of_id]]
  * [[ID.animation_data_create]]
  * [[ID.animation_data_clear]]
  * [[ID.update_tag]]
  * [[ID.preview_ensure]]
  * [[ID.bl_rna_get_subclass]]
  * [[ID.bl_rna_get_subclass_py]]

  
---|---  
  
## References

  * [[bpy.context.scene]]
  * [[BlendData.scenes]]
  * [[BlendDataScenes.new]]
  * [[BlendDataScenes.remove]]
  * [[Camera.view_frame]]
  * [[CompositorNodeCryptomatteV2.scene]]
  * [[CompositorNodeDefocus.scene]]
  * [[CompositorNodeRLayers.scene]]
  * [[Context.scene]]
  * [[Depsgraph.scene]]
  * [[Depsgraph.scene_eval]]
  * [[ID.override_hierarchy_create]]
  * [[IDOverrideLibrary.resync]]
  * [[Image.save_render]]

| 

  * [[Object.crazyspace_eval]]
  * [[Object.is_deform_modified]]
  * [[Object.is_modified]]
  * [[RenderEngine.bind_display_space_shader]]
  * [[RenderEngine.get_preview_pixel_size]]
  * [[RenderEngine.register_pass]]
  * [[RenderEngine.support_display_space_shader]]
  * [[RenderEngine.update_render_passes]]
  * `Scene.background_set`
  * [[SceneStrip.scene]]
  * [[StripsMeta.new_scene]]
  * [[StripsTopLevel.new_scene]]
  * [[Window.scene]]

  
---|---
