# Node(bpy_struct)

base class — [`bpy_struct`](bpy.types.bpy_struct.html#bpy.types.bpy_struct "bpy.types.bpy_struct")

subclasses — [`NodeCustomGroup`](bpy.types.NodeCustomGroup.html#bpy.types.NodeCustomGroup "bpy.types.NodeCustomGroup"), [`NodeInternal`](bpy.types.NodeInternal.html#bpy.types.NodeInternal "bpy.types.NodeInternal")

_class _bpy.types.Node(_bpy_struct_)
    

Node in a node tree

bl_description
    

Type:
    

string, default “”, (never None)

bl_height_default
    

Type:
    

float in [0, inf], default 0.0

bl_height_max
    

Type:
    

float in [0, inf], default 0.0

bl_height_min
    

Type:
    

float in [0, inf], default 0.0

bl_icon
    

The node icon

Type:
    

enum in [Icon Items](bpy_types_enum_items/icon_items.html#rna-enum-icon-items), default `'NODE'`

bl_idname
    

Type:
    

string, default “”, (never None)

bl_label
    

The node label

Type:
    

string, default “”, (never None)

bl_static_type
    

Legacy unique node type identifier, redundant with bl_idname property

Type:
    

string, default “”, (readonly, never None)

bl_width_default
    

Type:
    

float in [0, inf], default 0.0

bl_width_max
    

Type:
    

float in [0, inf], default 0.0

bl_width_min
    

Type:
    

float in [0, inf], default 0.0

color
    

Custom color of the node body

Type:
    

[`mathutils.Color`](mathutils.html#mathutils.Color "mathutils.Color") of 3 items in [0, 1], default (0.0, 0.0, 0.0)

color_tag
    

Node header color tag

  * `NONE` None – Default color tag for new nodes and node groups.

  * `ATTRIBUTE` Attribute.

  * `COLOR` Color.

  * `CONVERTER` Converter.

  * `DISTORT` Distort.

  * `FILTER` Filter.

  * `GEOMETRY` Geometry.

  * `INPUT` Input.

  * `MATTE` Matte.

  * `OUTPUT` Output.

  * `SCRIPT` Script.

  * `SHADER` Shader.

  * `TEXTURE` Texture.

  * `VECTOR` Vector.

  * `PATTERN` Pattern.

  * `INTERFACE` Interface.

  * `GROUP` Group.


Type:
    

enum in [`'NONE'`, `'ATTRIBUTE'`, `'COLOR'`, `'CONVERTER'`, `'DISTORT'`, `'FILTER'`, `'GEOMETRY'`, `'INPUT'`, `'MATTE'`, `'OUTPUT'`, `'SCRIPT'`, `'SHADER'`, `'TEXTURE'`, `'VECTOR'`, `'PATTERN'`, `'INTERFACE'`, `'GROUP'`], default `'NONE'`, (readonly)

dimensions
    

Absolute bounding box dimensions of the node

Type:
    

[`mathutils.Vector`](mathutils.html#mathutils.Vector "mathutils.Vector") of 2 items in [-inf, inf], default (0.0, 0.0), (readonly)

height
    

Height of the node

Type:
    

float in [-inf, inf], default 0.0

hide
    

Type:
    

boolean, default False

inputs
    

Type:
    

[`NodeInputs`](bpy.types.NodeInputs.html#bpy.types.NodeInputs "bpy.types.NodeInputs") [`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`NodeSocket`](bpy.types.NodeSocket.html#bpy.types.NodeSocket "bpy.types.NodeSocket"), (readonly)

internal_links
    

Internal input-to-output connections for muting

Type:
    

[`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`NodeLink`](bpy.types.NodeLink.html#bpy.types.NodeLink "bpy.types.NodeLink"), (readonly)

label
    

Optional custom node label

Type:
    

string, default “”, (never None)

location
    

Location of the node within its parent frame

Type:
    

[`mathutils.Vector`](mathutils.html#mathutils.Vector "mathutils.Vector") of 2 items in [-1e+06, 1e+06], default (0.0, 0.0)

location_absolute
    

Location of the node in the entire canvas

Type:
    

[`mathutils.Vector`](mathutils.html#mathutils.Vector "mathutils.Vector") of 2 items in [-1e+06, 1e+06], default (0.0, 0.0)

mute
    

Type:
    

boolean, default False

name
    

Unique node identifier

Type:
    

string, default “”, (never None)

outputs
    

Type:
    

[`NodeOutputs`](bpy.types.NodeOutputs.html#bpy.types.NodeOutputs "bpy.types.NodeOutputs") [`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`NodeSocket`](bpy.types.NodeSocket.html#bpy.types.NodeSocket "bpy.types.NodeSocket"), (readonly)

parent
    

Parent this node is attached to

Type:
    

`Node`

select
    

Node selection state

Type:
    

boolean, default False

show_options
    

Type:
    

boolean, default False

show_preview
    

Type:
    

boolean, default False

show_texture
    

Display node in viewport textured shading mode

Type:
    

boolean, default False

type
    

Legacy unique node type identifier, redundant with bl_idname property

Type:
    

string, default “”, (readonly, never None)

use_custom_color
    

Use custom color for the node

Type:
    

boolean, default False

warning_propagation
    

The kinds of messages that should be propagated from this node to the parent group node

Type:
    

enum in [`'ALL'`, `'NONE'`, `'ERRORS'`, `'ERRORS_AND_WARNINGS'`], default `'ALL'`

width
    

Width of the node

Type:
    

float in [-inf, inf], default 0.0

socket_value_update(_context_)
    

Update after property changes

_classmethod _is_registered_node_type()
    

True if a registered node type

Returns:
    

Result

Return type:
    

boolean

_classmethod _poll(_node_tree_)
    

If non-null output is returned, the node type can be added to the tree

Parameters:
    

**node_tree** ([`NodeTree`](bpy.types.NodeTree.html#bpy.types.NodeTree "bpy.types.NodeTree")) – Node Tree

Return type:
    

boolean

poll_instance(_node_tree_)
    

If non-null output is returned, the node can be added to the tree

Parameters:
    

**node_tree** ([`NodeTree`](bpy.types.NodeTree.html#bpy.types.NodeTree "bpy.types.NodeTree")) – Node Tree

Return type:
    

boolean

update()
    

Update on node graph topology changes (adding or removing nodes and links)

insert_link(_link_)
    

Handle creation of a link to or from the node

Parameters:
    

**link** ([`NodeLink`](bpy.types.NodeLink.html#bpy.types.NodeLink "bpy.types.NodeLink"), (never None)) – Link, Node link that will be inserted

init(_context_)
    

Initialize a new instance of this node

copy(_node_)
    

Initialize a new instance of this node from an existing node

Parameters:
    

**node** (`Node`, (never None)) – Node, Existing node to copy

free()
    

Clean up node on removal

draw_buttons(_context_ , _layout_)
    

Draw node buttons

Parameters:
    

**layout** ([`UILayout`](bpy.types.UILayout.html#bpy.types.UILayout "bpy.types.UILayout"), (never None)) – Layout, Layout in the UI

draw_buttons_ext(_context_ , _layout_)
    

Draw node buttons in the sidebar

Parameters:
    

**layout** ([`UILayout`](bpy.types.UILayout.html#bpy.types.UILayout "bpy.types.UILayout"), (never None)) – Layout, Layout in the UI

draw_label()
    

Returns a dynamic label string

Returns:
    

Label

Return type:
    

string, (never None)

debug_zone_body_lazy_function_graph()
    

Get the internal lazy-function graph for the body of this zone

Returns:
    

Dot Graph, Graph in dot format

Return type:
    

string

debug_zone_lazy_function_graph()
    

Get the internal lazy-function graph for this zone

Returns:
    

Dot Graph, Graph in dot format

Return type:
    

string

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

  * [`bpy.context.active_node`](bpy.context.html#bpy.context.active_node "bpy.context.active_node")
  * [`bpy.context.selected_nodes`](bpy.context.html#bpy.context.selected_nodes "bpy.context.selected_nodes")
  * [`bpy.context.texture_node`](bpy.context.html#bpy.context.texture_node "bpy.context.texture_node")
  * [`GeometryNodeClosureInput.paired_output`](bpy.types.GeometryNodeClosureInput.html#bpy.types.GeometryNodeClosureInput.paired_output "bpy.types.GeometryNodeClosureInput.paired_output")
  * [`GeometryNodeForeachGeometryElementInput.paired_output`](bpy.types.GeometryNodeForeachGeometryElementInput.html#bpy.types.GeometryNodeForeachGeometryElementInput.paired_output "bpy.types.GeometryNodeForeachGeometryElementInput.paired_output")
  * [`GeometryNodeMenuSwitch.enum_definition`](bpy.types.GeometryNodeMenuSwitch.html#bpy.types.GeometryNodeMenuSwitch.enum_definition "bpy.types.GeometryNodeMenuSwitch.enum_definition")
  * [`GeometryNodeRepeatInput.paired_output`](bpy.types.GeometryNodeRepeatInput.html#bpy.types.GeometryNodeRepeatInput.paired_output "bpy.types.GeometryNodeRepeatInput.paired_output")
  * [`GeometryNodeSimulationInput.paired_output`](bpy.types.GeometryNodeSimulationInput.html#bpy.types.GeometryNodeSimulationInput.paired_output "bpy.types.GeometryNodeSimulationInput.paired_output")
  * `Node.copy`
  * `Node.parent`
  * [`NodeLink.from_node`](bpy.types.NodeLink.html#bpy.types.NodeLink.from_node "bpy.types.NodeLink.from_node")
  * [`NodeLink.to_node`](bpy.types.NodeLink.html#bpy.types.NodeLink.to_node "bpy.types.NodeLink.to_node")
  * [`NodeSocket.draw`](bpy.types.NodeSocket.html#bpy.types.NodeSocket.draw "bpy.types.NodeSocket.draw")
  * [`NodeSocket.draw_color`](bpy.types.NodeSocket.html#bpy.types.NodeSocket.draw_color "bpy.types.NodeSocket.draw_color")
  * [`NodeSocket.node`](bpy.types.NodeSocket.html#bpy.types.NodeSocket.node "bpy.types.NodeSocket.node")
  * [`NodeSocketStandard.draw`](bpy.types.NodeSocketStandard.html#bpy.types.NodeSocketStandard.draw "bpy.types.NodeSocketStandard.draw")
  * [`NodeSocketStandard.draw_color`](bpy.types.NodeSocketStandard.html#bpy.types.NodeSocketStandard.draw_color "bpy.types.NodeSocketStandard.draw_color")
  * [`NodeTree.nodes`](bpy.types.NodeTree.html#bpy.types.NodeTree.nodes "bpy.types.NodeTree.nodes")
  * [`NodeTreeInterfaceSocket.from_socket`](bpy.types.NodeTreeInterfaceSocket.html#bpy.types.NodeTreeInterfaceSocket.from_socket "bpy.types.NodeTreeInterfaceSocket.from_socket")
  * [`NodeTreeInterfaceSocket.init_socket`](bpy.types.NodeTreeInterfaceSocket.html#bpy.types.NodeTreeInterfaceSocket.init_socket "bpy.types.NodeTreeInterfaceSocket.init_socket")
  * [`NodeTreeInterfaceSocketBool.from_socket`](bpy.types.NodeTreeInterfaceSocketBool.html#bpy.types.NodeTreeInterfaceSocketBool.from_socket "bpy.types.NodeTreeInterfaceSocketBool.from_socket")
  * [`NodeTreeInterfaceSocketBool.init_socket`](bpy.types.NodeTreeInterfaceSocketBool.html#bpy.types.NodeTreeInterfaceSocketBool.init_socket "bpy.types.NodeTreeInterfaceSocketBool.init_socket")
  * [`NodeTreeInterfaceSocketBundle.from_socket`](bpy.types.NodeTreeInterfaceSocketBundle.html#bpy.types.NodeTreeInterfaceSocketBundle.from_socket "bpy.types.NodeTreeInterfaceSocketBundle.from_socket")
  * [`NodeTreeInterfaceSocketBundle.init_socket`](bpy.types.NodeTreeInterfaceSocketBundle.html#bpy.types.NodeTreeInterfaceSocketBundle.init_socket "bpy.types.NodeTreeInterfaceSocketBundle.init_socket")
  * [`NodeTreeInterfaceSocketClosure.from_socket`](bpy.types.NodeTreeInterfaceSocketClosure.html#bpy.types.NodeTreeInterfaceSocketClosure.from_socket "bpy.types.NodeTreeInterfaceSocketClosure.from_socket")
  * [`NodeTreeInterfaceSocketClosure.init_socket`](bpy.types.NodeTreeInterfaceSocketClosure.html#bpy.types.NodeTreeInterfaceSocketClosure.init_socket "bpy.types.NodeTreeInterfaceSocketClosure.init_socket")
  * [`NodeTreeInterfaceSocketCollection.from_socket`](bpy.types.NodeTreeInterfaceSocketCollection.html#bpy.types.NodeTreeInterfaceSocketCollection.from_socket "bpy.types.NodeTreeInterfaceSocketCollection.from_socket")
  * [`NodeTreeInterfaceSocketCollection.init_socket`](bpy.types.NodeTreeInterfaceSocketCollection.html#bpy.types.NodeTreeInterfaceSocketCollection.init_socket "bpy.types.NodeTreeInterfaceSocketCollection.init_socket")
  * [`NodeTreeInterfaceSocketColor.from_socket`](bpy.types.NodeTreeInterfaceSocketColor.html#bpy.types.NodeTreeInterfaceSocketColor.from_socket "bpy.types.NodeTreeInterfaceSocketColor.from_socket")
  * [`NodeTreeInterfaceSocketColor.init_socket`](bpy.types.NodeTreeInterfaceSocketColor.html#bpy.types.NodeTreeInterfaceSocketColor.init_socket "bpy.types.NodeTreeInterfaceSocketColor.init_socket")
  * [`NodeTreeInterfaceSocketFloat.from_socket`](bpy.types.NodeTreeInterfaceSocketFloat.html#bpy.types.NodeTreeInterfaceSocketFloat.from_socket "bpy.types.NodeTreeInterfaceSocketFloat.from_socket")
  * [`NodeTreeInterfaceSocketFloat.init_socket`](bpy.types.NodeTreeInterfaceSocketFloat.html#bpy.types.NodeTreeInterfaceSocketFloat.init_socket "bpy.types.NodeTreeInterfaceSocketFloat.init_socket")
  * [`NodeTreeInterfaceSocketFloatAngle.from_socket`](bpy.types.NodeTreeInterfaceSocketFloatAngle.html#bpy.types.NodeTreeInterfaceSocketFloatAngle.from_socket "bpy.types.NodeTreeInterfaceSocketFloatAngle.from_socket")
  * [`NodeTreeInterfaceSocketFloatAngle.init_socket`](bpy.types.NodeTreeInterfaceSocketFloatAngle.html#bpy.types.NodeTreeInterfaceSocketFloatAngle.init_socket "bpy.types.NodeTreeInterfaceSocketFloatAngle.init_socket")
  * [`NodeTreeInterfaceSocketFloatColorTemperature.from_socket`](bpy.types.NodeTreeInterfaceSocketFloatColorTemperature.html#bpy.types.NodeTreeInterfaceSocketFloatColorTemperature.from_socket "bpy.types.NodeTreeInterfaceSocketFloatColorTemperature.from_socket")
  * [`NodeTreeInterfaceSocketFloatColorTemperature.init_socket`](bpy.types.NodeTreeInterfaceSocketFloatColorTemperature.html#bpy.types.NodeTreeInterfaceSocketFloatColorTemperature.init_socket "bpy.types.NodeTreeInterfaceSocketFloatColorTemperature.init_socket")
  * [`NodeTreeInterfaceSocketFloatDistance.from_socket`](bpy.types.NodeTreeInterfaceSocketFloatDistance.html#bpy.types.NodeTreeInterfaceSocketFloatDistance.from_socket "bpy.types.NodeTreeInterfaceSocketFloatDistance.from_socket")
  * [`NodeTreeInterfaceSocketFloatDistance.init_socket`](bpy.types.NodeTreeInterfaceSocketFloatDistance.html#bpy.types.NodeTreeInterfaceSocketFloatDistance.init_socket "bpy.types.NodeTreeInterfaceSocketFloatDistance.init_socket")
  * [`NodeTreeInterfaceSocketFloatFactor.from_socket`](bpy.types.NodeTreeInterfaceSocketFloatFactor.html#bpy.types.NodeTreeInterfaceSocketFloatFactor.from_socket "bpy.types.NodeTreeInterfaceSocketFloatFactor.from_socket")
  * [`NodeTreeInterfaceSocketFloatFactor.init_socket`](bpy.types.NodeTreeInterfaceSocketFloatFactor.html#bpy.types.NodeTreeInterfaceSocketFloatFactor.init_socket "bpy.types.NodeTreeInterfaceSocketFloatFactor.init_socket")
  * [`NodeTreeInterfaceSocketFloatFrequency.from_socket`](bpy.types.NodeTreeInterfaceSocketFloatFrequency.html#bpy.types.NodeTreeInterfaceSocketFloatFrequency.from_socket "bpy.types.NodeTreeInterfaceSocketFloatFrequency.from_socket")
  * [`NodeTreeInterfaceSocketFloatFrequency.init_socket`](bpy.types.NodeTreeInterfaceSocketFloatFrequency.html#bpy.types.NodeTreeInterfaceSocketFloatFrequency.init_socket "bpy.types.NodeTreeInterfaceSocketFloatFrequency.init_socket")
  * [`NodeTreeInterfaceSocketFloatPercentage.from_socket`](bpy.types.NodeTreeInterfaceSocketFloatPercentage.html#bpy.types.NodeTreeInterfaceSocketFloatPercentage.from_socket "bpy.types.NodeTreeInterfaceSocketFloatPercentage.from_socket")
  * [`NodeTreeInterfaceSocketFloatPercentage.init_socket`](bpy.types.NodeTreeInterfaceSocketFloatPercentage.html#bpy.types.NodeTreeInterfaceSocketFloatPercentage.init_socket "bpy.types.NodeTreeInterfaceSocketFloatPercentage.init_socket")
  * [`NodeTreeInterfaceSocketFloatTime.from_socket`](bpy.types.NodeTreeInterfaceSocketFloatTime.html#bpy.types.NodeTreeInterfaceSocketFloatTime.from_socket "bpy.types.NodeTreeInterfaceSocketFloatTime.from_socket")
  * [`NodeTreeInterfaceSocketFloatTime.init_socket`](bpy.types.NodeTreeInterfaceSocketFloatTime.html#bpy.types.NodeTreeInterfaceSocketFloatTime.init_socket "bpy.types.NodeTreeInterfaceSocketFloatTime.init_socket")
  * [`NodeTreeInterfaceSocketFloatTimeAbsolute.from_socket`](bpy.types.NodeTreeInterfaceSocketFloatTimeAbsolute.html#bpy.types.NodeTreeInterfaceSocketFloatTimeAbsolute.from_socket "bpy.types.NodeTreeInterfaceSocketFloatTimeAbsolute.from_socket")
  * [`NodeTreeInterfaceSocketFloatTimeAbsolute.init_socket`](bpy.types.NodeTreeInterfaceSocketFloatTimeAbsolute.html#bpy.types.NodeTreeInterfaceSocketFloatTimeAbsolute.init_socket "bpy.types.NodeTreeInterfaceSocketFloatTimeAbsolute.init_socket")
  * [`NodeTreeInterfaceSocketFloatUnsigned.from_socket`](bpy.types.NodeTreeInterfaceSocketFloatUnsigned.html#bpy.types.NodeTreeInterfaceSocketFloatUnsigned.from_socket "bpy.types.NodeTreeInterfaceSocketFloatUnsigned.from_socket")
  * [`NodeTreeInterfaceSocketFloatUnsigned.init_socket`](bpy.types.NodeTreeInterfaceSocketFloatUnsigned.html#bpy.types.NodeTreeInterfaceSocketFloatUnsigned.init_socket "bpy.types.NodeTreeInterfaceSocketFloatUnsigned.init_socket")
  * [`NodeTreeInterfaceSocketFloatWavelength.from_socket`](bpy.types.NodeTreeInterfaceSocketFloatWavelength.html#bpy.types.NodeTreeInterfaceSocketFloatWavelength.from_socket "bpy.types.NodeTreeInterfaceSocketFloatWavelength.from_socket")
  * [`NodeTreeInterfaceSocketFloatWavelength.init_socket`](bpy.types.NodeTreeInterfaceSocketFloatWavelength.html#bpy.types.NodeTreeInterfaceSocketFloatWavelength.init_socket "bpy.types.NodeTreeInterfaceSocketFloatWavelength.init_socket")
  * [`NodeTreeInterfaceSocketGeometry.from_socket`](bpy.types.NodeTreeInterfaceSocketGeometry.html#bpy.types.NodeTreeInterfaceSocketGeometry.from_socket "bpy.types.NodeTreeInterfaceSocketGeometry.from_socket")
  * [`NodeTreeInterfaceSocketGeometry.init_socket`](bpy.types.NodeTreeInterfaceSocketGeometry.html#bpy.types.NodeTreeInterfaceSocketGeometry.init_socket "bpy.types.NodeTreeInterfaceSocketGeometry.init_socket")
  * [`NodeTreeInterfaceSocketImage.from_socket`](bpy.types.NodeTreeInterfaceSocketImage.html#bpy.types.NodeTreeInterfaceSocketImage.from_socket "bpy.types.NodeTreeInterfaceSocketImage.from_socket")
  * [`NodeTreeInterfaceSocketImage.init_socket`](bpy.types.NodeTreeInterfaceSocketImage.html#bpy.types.NodeTreeInterfaceSocketImage.init_socket "bpy.types.NodeTreeInterfaceSocketImage.init_socket")
  * [`NodeTreeInterfaceSocketInt.from_socket`](bpy.types.NodeTreeInterfaceSocketInt.html#bpy.types.NodeTreeInterfaceSocketInt.from_socket "bpy.types.NodeTreeInterfaceSocketInt.from_socket")
  * [`NodeTreeInterfaceSocketInt.init_socket`](bpy.types.NodeTreeInterfaceSocketInt.html#bpy.types.NodeTreeInterfaceSocketInt.init_socket "bpy.types.NodeTreeInterfaceSocketInt.init_socket")
  * [`NodeTreeInterfaceSocketIntFactor.from_socket`](bpy.types.NodeTreeInterfaceSocketIntFactor.html#bpy.types.NodeTreeInterfaceSocketIntFactor.from_socket "bpy.types.NodeTreeInterfaceSocketIntFactor.from_socket")
  * [`NodeTreeInterfaceSocketIntFactor.init_socket`](bpy.types.NodeTreeInterfaceSocketIntFactor.html#bpy.types.NodeTreeInterfaceSocketIntFactor.init_socket "bpy.types.NodeTreeInterfaceSocketIntFactor.init_socket")
  * [`NodeTreeInterfaceSocketIntPercentage.from_socket`](bpy.types.NodeTreeInterfaceSocketIntPercentage.html#bpy.types.NodeTreeInterfaceSocketIntPercentage.from_socket "bpy.types.NodeTreeInterfaceSocketIntPercentage.from_socket")
  * [`NodeTreeInterfaceSocketIntPercentage.init_socket`](bpy.types.NodeTreeInterfaceSocketIntPercentage.html#bpy.types.NodeTreeInterfaceSocketIntPercentage.init_socket "bpy.types.NodeTreeInterfaceSocketIntPercentage.init_socket")
  * [`NodeTreeInterfaceSocketIntUnsigned.from_socket`](bpy.types.NodeTreeInterfaceSocketIntUnsigned.html#bpy.types.NodeTreeInterfaceSocketIntUnsigned.from_socket "bpy.types.NodeTreeInterfaceSocketIntUnsigned.from_socket")
  * [`NodeTreeInterfaceSocketIntUnsigned.init_socket`](bpy.types.NodeTreeInterfaceSocketIntUnsigned.html#bpy.types.NodeTreeInterfaceSocketIntUnsigned.init_socket "bpy.types.NodeTreeInterfaceSocketIntUnsigned.init_socket")
  * [`NodeTreeInterfaceSocketMaterial.from_socket`](bpy.types.NodeTreeInterfaceSocketMaterial.html#bpy.types.NodeTreeInterfaceSocketMaterial.from_socket "bpy.types.NodeTreeInterfaceSocketMaterial.from_socket")
  * [`NodeTreeInterfaceSocketMaterial.init_socket`](bpy.types.NodeTreeInterfaceSocketMaterial.html#bpy.types.NodeTreeInterfaceSocketMaterial.init_socket "bpy.types.NodeTreeInterfaceSocketMaterial.init_socket")
  * [`NodeTreeInterfaceSocketMatrix.from_socket`](bpy.types.NodeTreeInterfaceSocketMatrix.html#bpy.types.NodeTreeInterfaceSocketMatrix.from_socket "bpy.types.NodeTreeInterfaceSocketMatrix.from_socket")
  * [`NodeTreeInterfaceSocketMatrix.init_socket`](bpy.types.NodeTreeInterfaceSocketMatrix.html#bpy.types.NodeTreeInterfaceSocketMatrix.init_socket "bpy.types.NodeTreeInterfaceSocketMatrix.init_socket")
  * [`NodeTreeInterfaceSocketMenu.from_socket`](bpy.types.NodeTreeInterfaceSocketMenu.html#bpy.types.NodeTreeInterfaceSocketMenu.from_socket "bpy.types.NodeTreeInterfaceSocketMenu.from_socket")
  * [`NodeTreeInterfaceSocketMenu.init_socket`](bpy.types.NodeTreeInterfaceSocketMenu.html#bpy.types.NodeTreeInterfaceSocketMenu.init_socket "bpy.types.NodeTreeInterfaceSocketMenu.init_socket")
  * [`NodeTreeInterfaceSocketObject.from_socket`](bpy.types.NodeTreeInterfaceSocketObject.html#bpy.types.NodeTreeInterfaceSocketObject.from_socket "bpy.types.NodeTreeInterfaceSocketObject.from_socket")
  * [`NodeTreeInterfaceSocketObject.init_socket`](bpy.types.NodeTreeInterfaceSocketObject.html#bpy.types.NodeTreeInterfaceSocketObject.init_socket "bpy.types.NodeTreeInterfaceSocketObject.init_socket")
  * [`NodeTreeInterfaceSocketRotation.from_socket`](bpy.types.NodeTreeInterfaceSocketRotation.html#bpy.types.NodeTreeInterfaceSocketRotation.from_socket "bpy.types.NodeTreeInterfaceSocketRotation.from_socket")

| 

  * [`NodeTreeInterfaceSocketRotation.init_socket`](bpy.types.NodeTreeInterfaceSocketRotation.html#bpy.types.NodeTreeInterfaceSocketRotation.init_socket "bpy.types.NodeTreeInterfaceSocketRotation.init_socket")
  * [`NodeTreeInterfaceSocketShader.from_socket`](bpy.types.NodeTreeInterfaceSocketShader.html#bpy.types.NodeTreeInterfaceSocketShader.from_socket "bpy.types.NodeTreeInterfaceSocketShader.from_socket")
  * [`NodeTreeInterfaceSocketShader.init_socket`](bpy.types.NodeTreeInterfaceSocketShader.html#bpy.types.NodeTreeInterfaceSocketShader.init_socket "bpy.types.NodeTreeInterfaceSocketShader.init_socket")
  * [`NodeTreeInterfaceSocketString.from_socket`](bpy.types.NodeTreeInterfaceSocketString.html#bpy.types.NodeTreeInterfaceSocketString.from_socket "bpy.types.NodeTreeInterfaceSocketString.from_socket")
  * [`NodeTreeInterfaceSocketString.init_socket`](bpy.types.NodeTreeInterfaceSocketString.html#bpy.types.NodeTreeInterfaceSocketString.init_socket "bpy.types.NodeTreeInterfaceSocketString.init_socket")
  * [`NodeTreeInterfaceSocketStringFilePath.from_socket`](bpy.types.NodeTreeInterfaceSocketStringFilePath.html#bpy.types.NodeTreeInterfaceSocketStringFilePath.from_socket "bpy.types.NodeTreeInterfaceSocketStringFilePath.from_socket")
  * [`NodeTreeInterfaceSocketStringFilePath.init_socket`](bpy.types.NodeTreeInterfaceSocketStringFilePath.html#bpy.types.NodeTreeInterfaceSocketStringFilePath.init_socket "bpy.types.NodeTreeInterfaceSocketStringFilePath.init_socket")
  * [`NodeTreeInterfaceSocketTexture.from_socket`](bpy.types.NodeTreeInterfaceSocketTexture.html#bpy.types.NodeTreeInterfaceSocketTexture.from_socket "bpy.types.NodeTreeInterfaceSocketTexture.from_socket")
  * [`NodeTreeInterfaceSocketTexture.init_socket`](bpy.types.NodeTreeInterfaceSocketTexture.html#bpy.types.NodeTreeInterfaceSocketTexture.init_socket "bpy.types.NodeTreeInterfaceSocketTexture.init_socket")
  * [`NodeTreeInterfaceSocketVector.from_socket`](bpy.types.NodeTreeInterfaceSocketVector.html#bpy.types.NodeTreeInterfaceSocketVector.from_socket "bpy.types.NodeTreeInterfaceSocketVector.from_socket")
  * [`NodeTreeInterfaceSocketVector.init_socket`](bpy.types.NodeTreeInterfaceSocketVector.html#bpy.types.NodeTreeInterfaceSocketVector.init_socket "bpy.types.NodeTreeInterfaceSocketVector.init_socket")
  * [`NodeTreeInterfaceSocketVector2D.from_socket`](bpy.types.NodeTreeInterfaceSocketVector2D.html#bpy.types.NodeTreeInterfaceSocketVector2D.from_socket "bpy.types.NodeTreeInterfaceSocketVector2D.from_socket")
  * [`NodeTreeInterfaceSocketVector2D.init_socket`](bpy.types.NodeTreeInterfaceSocketVector2D.html#bpy.types.NodeTreeInterfaceSocketVector2D.init_socket "bpy.types.NodeTreeInterfaceSocketVector2D.init_socket")
  * [`NodeTreeInterfaceSocketVector4D.from_socket`](bpy.types.NodeTreeInterfaceSocketVector4D.html#bpy.types.NodeTreeInterfaceSocketVector4D.from_socket "bpy.types.NodeTreeInterfaceSocketVector4D.from_socket")
  * [`NodeTreeInterfaceSocketVector4D.init_socket`](bpy.types.NodeTreeInterfaceSocketVector4D.html#bpy.types.NodeTreeInterfaceSocketVector4D.init_socket "bpy.types.NodeTreeInterfaceSocketVector4D.init_socket")
  * [`NodeTreeInterfaceSocketVectorAcceleration.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorAcceleration.html#bpy.types.NodeTreeInterfaceSocketVectorAcceleration.from_socket "bpy.types.NodeTreeInterfaceSocketVectorAcceleration.from_socket")
  * [`NodeTreeInterfaceSocketVectorAcceleration.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorAcceleration.html#bpy.types.NodeTreeInterfaceSocketVectorAcceleration.init_socket "bpy.types.NodeTreeInterfaceSocketVectorAcceleration.init_socket")
  * [`NodeTreeInterfaceSocketVectorAcceleration2D.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorAcceleration2D.html#bpy.types.NodeTreeInterfaceSocketVectorAcceleration2D.from_socket "bpy.types.NodeTreeInterfaceSocketVectorAcceleration2D.from_socket")
  * [`NodeTreeInterfaceSocketVectorAcceleration2D.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorAcceleration2D.html#bpy.types.NodeTreeInterfaceSocketVectorAcceleration2D.init_socket "bpy.types.NodeTreeInterfaceSocketVectorAcceleration2D.init_socket")
  * [`NodeTreeInterfaceSocketVectorAcceleration4D.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorAcceleration4D.html#bpy.types.NodeTreeInterfaceSocketVectorAcceleration4D.from_socket "bpy.types.NodeTreeInterfaceSocketVectorAcceleration4D.from_socket")
  * [`NodeTreeInterfaceSocketVectorAcceleration4D.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorAcceleration4D.html#bpy.types.NodeTreeInterfaceSocketVectorAcceleration4D.init_socket "bpy.types.NodeTreeInterfaceSocketVectorAcceleration4D.init_socket")
  * [`NodeTreeInterfaceSocketVectorDirection.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorDirection.html#bpy.types.NodeTreeInterfaceSocketVectorDirection.from_socket "bpy.types.NodeTreeInterfaceSocketVectorDirection.from_socket")
  * [`NodeTreeInterfaceSocketVectorDirection.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorDirection.html#bpy.types.NodeTreeInterfaceSocketVectorDirection.init_socket "bpy.types.NodeTreeInterfaceSocketVectorDirection.init_socket")
  * [`NodeTreeInterfaceSocketVectorDirection2D.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorDirection2D.html#bpy.types.NodeTreeInterfaceSocketVectorDirection2D.from_socket "bpy.types.NodeTreeInterfaceSocketVectorDirection2D.from_socket")
  * [`NodeTreeInterfaceSocketVectorDirection2D.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorDirection2D.html#bpy.types.NodeTreeInterfaceSocketVectorDirection2D.init_socket "bpy.types.NodeTreeInterfaceSocketVectorDirection2D.init_socket")
  * [`NodeTreeInterfaceSocketVectorDirection4D.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorDirection4D.html#bpy.types.NodeTreeInterfaceSocketVectorDirection4D.from_socket "bpy.types.NodeTreeInterfaceSocketVectorDirection4D.from_socket")
  * [`NodeTreeInterfaceSocketVectorDirection4D.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorDirection4D.html#bpy.types.NodeTreeInterfaceSocketVectorDirection4D.init_socket "bpy.types.NodeTreeInterfaceSocketVectorDirection4D.init_socket")
  * [`NodeTreeInterfaceSocketVectorEuler.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorEuler.html#bpy.types.NodeTreeInterfaceSocketVectorEuler.from_socket "bpy.types.NodeTreeInterfaceSocketVectorEuler.from_socket")
  * [`NodeTreeInterfaceSocketVectorEuler.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorEuler.html#bpy.types.NodeTreeInterfaceSocketVectorEuler.init_socket "bpy.types.NodeTreeInterfaceSocketVectorEuler.init_socket")
  * [`NodeTreeInterfaceSocketVectorEuler2D.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorEuler2D.html#bpy.types.NodeTreeInterfaceSocketVectorEuler2D.from_socket "bpy.types.NodeTreeInterfaceSocketVectorEuler2D.from_socket")
  * [`NodeTreeInterfaceSocketVectorEuler2D.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorEuler2D.html#bpy.types.NodeTreeInterfaceSocketVectorEuler2D.init_socket "bpy.types.NodeTreeInterfaceSocketVectorEuler2D.init_socket")
  * [`NodeTreeInterfaceSocketVectorEuler4D.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorEuler4D.html#bpy.types.NodeTreeInterfaceSocketVectorEuler4D.from_socket "bpy.types.NodeTreeInterfaceSocketVectorEuler4D.from_socket")
  * [`NodeTreeInterfaceSocketVectorEuler4D.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorEuler4D.html#bpy.types.NodeTreeInterfaceSocketVectorEuler4D.init_socket "bpy.types.NodeTreeInterfaceSocketVectorEuler4D.init_socket")
  * [`NodeTreeInterfaceSocketVectorFactor.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorFactor.html#bpy.types.NodeTreeInterfaceSocketVectorFactor.from_socket "bpy.types.NodeTreeInterfaceSocketVectorFactor.from_socket")
  * [`NodeTreeInterfaceSocketVectorFactor.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorFactor.html#bpy.types.NodeTreeInterfaceSocketVectorFactor.init_socket "bpy.types.NodeTreeInterfaceSocketVectorFactor.init_socket")
  * [`NodeTreeInterfaceSocketVectorFactor2D.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorFactor2D.html#bpy.types.NodeTreeInterfaceSocketVectorFactor2D.from_socket "bpy.types.NodeTreeInterfaceSocketVectorFactor2D.from_socket")
  * [`NodeTreeInterfaceSocketVectorFactor2D.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorFactor2D.html#bpy.types.NodeTreeInterfaceSocketVectorFactor2D.init_socket "bpy.types.NodeTreeInterfaceSocketVectorFactor2D.init_socket")
  * [`NodeTreeInterfaceSocketVectorFactor4D.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorFactor4D.html#bpy.types.NodeTreeInterfaceSocketVectorFactor4D.from_socket "bpy.types.NodeTreeInterfaceSocketVectorFactor4D.from_socket")
  * [`NodeTreeInterfaceSocketVectorFactor4D.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorFactor4D.html#bpy.types.NodeTreeInterfaceSocketVectorFactor4D.init_socket "bpy.types.NodeTreeInterfaceSocketVectorFactor4D.init_socket")
  * [`NodeTreeInterfaceSocketVectorPercentage.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorPercentage.html#bpy.types.NodeTreeInterfaceSocketVectorPercentage.from_socket "bpy.types.NodeTreeInterfaceSocketVectorPercentage.from_socket")
  * [`NodeTreeInterfaceSocketVectorPercentage.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorPercentage.html#bpy.types.NodeTreeInterfaceSocketVectorPercentage.init_socket "bpy.types.NodeTreeInterfaceSocketVectorPercentage.init_socket")
  * [`NodeTreeInterfaceSocketVectorPercentage2D.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorPercentage2D.html#bpy.types.NodeTreeInterfaceSocketVectorPercentage2D.from_socket "bpy.types.NodeTreeInterfaceSocketVectorPercentage2D.from_socket")
  * [`NodeTreeInterfaceSocketVectorPercentage2D.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorPercentage2D.html#bpy.types.NodeTreeInterfaceSocketVectorPercentage2D.init_socket "bpy.types.NodeTreeInterfaceSocketVectorPercentage2D.init_socket")
  * [`NodeTreeInterfaceSocketVectorPercentage4D.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorPercentage4D.html#bpy.types.NodeTreeInterfaceSocketVectorPercentage4D.from_socket "bpy.types.NodeTreeInterfaceSocketVectorPercentage4D.from_socket")
  * [`NodeTreeInterfaceSocketVectorPercentage4D.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorPercentage4D.html#bpy.types.NodeTreeInterfaceSocketVectorPercentage4D.init_socket "bpy.types.NodeTreeInterfaceSocketVectorPercentage4D.init_socket")
  * [`NodeTreeInterfaceSocketVectorTranslation.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorTranslation.html#bpy.types.NodeTreeInterfaceSocketVectorTranslation.from_socket "bpy.types.NodeTreeInterfaceSocketVectorTranslation.from_socket")
  * [`NodeTreeInterfaceSocketVectorTranslation.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorTranslation.html#bpy.types.NodeTreeInterfaceSocketVectorTranslation.init_socket "bpy.types.NodeTreeInterfaceSocketVectorTranslation.init_socket")
  * [`NodeTreeInterfaceSocketVectorTranslation2D.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorTranslation2D.html#bpy.types.NodeTreeInterfaceSocketVectorTranslation2D.from_socket "bpy.types.NodeTreeInterfaceSocketVectorTranslation2D.from_socket")
  * [`NodeTreeInterfaceSocketVectorTranslation2D.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorTranslation2D.html#bpy.types.NodeTreeInterfaceSocketVectorTranslation2D.init_socket "bpy.types.NodeTreeInterfaceSocketVectorTranslation2D.init_socket")
  * [`NodeTreeInterfaceSocketVectorTranslation4D.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorTranslation4D.html#bpy.types.NodeTreeInterfaceSocketVectorTranslation4D.from_socket "bpy.types.NodeTreeInterfaceSocketVectorTranslation4D.from_socket")
  * [`NodeTreeInterfaceSocketVectorTranslation4D.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorTranslation4D.html#bpy.types.NodeTreeInterfaceSocketVectorTranslation4D.init_socket "bpy.types.NodeTreeInterfaceSocketVectorTranslation4D.init_socket")
  * [`NodeTreeInterfaceSocketVectorVelocity.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorVelocity.html#bpy.types.NodeTreeInterfaceSocketVectorVelocity.from_socket "bpy.types.NodeTreeInterfaceSocketVectorVelocity.from_socket")
  * [`NodeTreeInterfaceSocketVectorVelocity.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorVelocity.html#bpy.types.NodeTreeInterfaceSocketVectorVelocity.init_socket "bpy.types.NodeTreeInterfaceSocketVectorVelocity.init_socket")
  * [`NodeTreeInterfaceSocketVectorVelocity2D.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorVelocity2D.html#bpy.types.NodeTreeInterfaceSocketVectorVelocity2D.from_socket "bpy.types.NodeTreeInterfaceSocketVectorVelocity2D.from_socket")
  * [`NodeTreeInterfaceSocketVectorVelocity2D.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorVelocity2D.html#bpy.types.NodeTreeInterfaceSocketVectorVelocity2D.init_socket "bpy.types.NodeTreeInterfaceSocketVectorVelocity2D.init_socket")
  * [`NodeTreeInterfaceSocketVectorVelocity4D.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorVelocity4D.html#bpy.types.NodeTreeInterfaceSocketVectorVelocity4D.from_socket "bpy.types.NodeTreeInterfaceSocketVectorVelocity4D.from_socket")
  * [`NodeTreeInterfaceSocketVectorVelocity4D.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorVelocity4D.html#bpy.types.NodeTreeInterfaceSocketVectorVelocity4D.init_socket "bpy.types.NodeTreeInterfaceSocketVectorVelocity4D.init_socket")
  * [`NodeTreeInterfaceSocketVectorXYZ.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorXYZ.html#bpy.types.NodeTreeInterfaceSocketVectorXYZ.from_socket "bpy.types.NodeTreeInterfaceSocketVectorXYZ.from_socket")
  * [`NodeTreeInterfaceSocketVectorXYZ.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorXYZ.html#bpy.types.NodeTreeInterfaceSocketVectorXYZ.init_socket "bpy.types.NodeTreeInterfaceSocketVectorXYZ.init_socket")
  * [`NodeTreeInterfaceSocketVectorXYZ2D.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorXYZ2D.html#bpy.types.NodeTreeInterfaceSocketVectorXYZ2D.from_socket "bpy.types.NodeTreeInterfaceSocketVectorXYZ2D.from_socket")
  * [`NodeTreeInterfaceSocketVectorXYZ2D.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorXYZ2D.html#bpy.types.NodeTreeInterfaceSocketVectorXYZ2D.init_socket "bpy.types.NodeTreeInterfaceSocketVectorXYZ2D.init_socket")
  * [`NodeTreeInterfaceSocketVectorXYZ4D.from_socket`](bpy.types.NodeTreeInterfaceSocketVectorXYZ4D.html#bpy.types.NodeTreeInterfaceSocketVectorXYZ4D.from_socket "bpy.types.NodeTreeInterfaceSocketVectorXYZ4D.from_socket")
  * [`NodeTreeInterfaceSocketVectorXYZ4D.init_socket`](bpy.types.NodeTreeInterfaceSocketVectorXYZ4D.html#bpy.types.NodeTreeInterfaceSocketVectorXYZ4D.init_socket "bpy.types.NodeTreeInterfaceSocketVectorXYZ4D.init_socket")
  * [`Nodes.active`](bpy.types.Nodes.html#bpy.types.Nodes.active "bpy.types.Nodes.active")
  * [`Nodes.new`](bpy.types.Nodes.html#bpy.types.Nodes.new "bpy.types.Nodes.new")
  * [`Nodes.remove`](bpy.types.Nodes.html#bpy.types.Nodes.remove "bpy.types.Nodes.remove")
  * [`NodesModifierBake.node`](bpy.types.NodesModifierBake.html#bpy.types.NodesModifierBake.node "bpy.types.NodesModifierBake.node")
  * [`RenderEngine.update_script_node`](bpy.types.RenderEngine.html#bpy.types.RenderEngine.update_script_node "bpy.types.RenderEngine.update_script_node")
  * [`SpaceNodeEditorPath.append`](bpy.types.SpaceNodeEditorPath.html#bpy.types.SpaceNodeEditorPath.append "bpy.types.SpaceNodeEditorPath.append")
  * [`UILayout.template_node_inputs`](bpy.types.UILayout.html#bpy.types.UILayout.template_node_inputs "bpy.types.UILayout.template_node_inputs")
  * [`UILayout.template_node_link`](bpy.types.UILayout.html#bpy.types.UILayout.template_node_link "bpy.types.UILayout.template_node_link")
  * [`UILayout.template_node_view`](bpy.types.UILayout.html#bpy.types.UILayout.template_node_view "bpy.types.UILayout.template_node_view")

  
---|---
