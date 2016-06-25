# SA:MP libraries for vehicles

Many useful libraries and systems for vehicles

#### Libraries list
* vh_data
* vh_sadata
* vh_utils
* vhs_label
* vhs_surfing

#### Functions list

| Library      /         Function                                 |                                                   Parameters                                                                                                                                                                                                                                                                                                                                                                                    | Returns value                    |
|:----------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|
| vh\_data     / AddStaticVehicle (_Hook_)                        | `modelid, Float:spawn_x, Float:spawn_y, Float:spawn_z, Float:z_angle, color1, color2`                                                                                                                                                                                                                                                                                                                                                           | vehicleid                        |
| vh\_data     / AddStaticVehicleEx (_Hook_)                      | `modelid, Float:spawn_x, Float:spawn_y, Float:spawn_z, Float:z_angle, color1, color2, respawn_delay, addsiren = 0`                                                                                                                                                                                                                                                                                                                              | vehicleid                        |
| vh\_data     / CreateVehicle (_Hook_)                           | `vehicletype, Float:x, Float:y, Float:z, Float:rotation, color1, color2, respawn_delay, addsiren = 0`                                                                                                                                                                                                                                                                                                                                           | vehicleid                        |
| vh\_data     / DestroyVehicle (_Hook_)                          | `vehicleid`                                                                                                                                                                                                                                                                                                                                                                                                                                     | **true** or **false**            |
| vh\_data     / SetVehicleToRespawn (_Hook_)                     | `vehicleid`                                                                                                                                                                                                                                                                                                                                                                                                                                     | **true** or **false**            |
| vh\_data     / SetVehicleVirtualWorld (_Hook_)                  | `vehicleid, worldid`                                                                                                                                                                                                                                                                                                                                                                                                                            | -                                |
| vh\_data     / GetVehicleColor                                  | `vehicleid, &color1, &color2`                                                                                                                                                                                                                                                                                                                                                                                                                   | **true** or **false**            |
| vh\_data     / SetVehicleColor (_Macros_)                       | `vehicleid, color1, color2`                                                                                                                                                                                                                                                                                                                                                                                                                     | -                                |
| vh\_data     / GetVehiclePaintjob                               | `vehicleid`                                                                                                                                                                                                                                                                                                                                                                                                                                     | `INVALID_VEHICLE_ID` or paintjob |
| vh\_data     / SetVehiclePaintjob                               | `vehicleid, paintjobid`                                                                                                                                                                                                                                                                                                                                                                                                                         | `INVALID_VEHICLE_ID` or 1 or 0   |
| vh\_data     / GetVehicleInterior                               | `vehicleid`                                                                                                                                                                                                                                                                                                                                                                                                                                     | `INVALID_VEHICLE_ID` or interior |
| vh\_data     / SetVehicleInterior                               | `vehicleid, interiorid`                                                                                                                                                                                                                                                                                                                                                                                                                         | `INVALID_VEHICLE_ID` or 1 or 0   |
| vh\_data     / GetVehicleLastDriver                             | `vehicleid`                                                                                                                                                                                                                                                                                                                                                                                                                                     | `INVALID_PLAYER_ID`  or playerid |
| vh\_data     / IsVehicleBlown                                   | `vehicleid`                                                                                                                                                                                                                                                                                                                                                                                                                                     | **true** or **false**            |
| vh\_data     / AttachTrailerToVehicle (_Hook_)                  | `trailerid, vehicleid`                                                                                                                                                                                                                                                                                                                                                                                                                          | **true** or **false**            |
| vh\_sadata   / GetModelStaticSpeed                              | `modelid`                                                                                                                                                                                                                                                                                                                                                                                                                                       | -1 or vehicle Max speed          |
| vh\_sadata   / GetModelStaticIdFromName                         | `const name[]`                                                                                                                                                                                                                                                                                                                                                                                                                                  | 0 or modelid                     |
| vh\_sadata   / GetModelStaticNameFromId                         | `modelid, name[]`                                                                                                                                                                                                                                                                                                                                                                                                                               | 0 or name length                 |
| vh\_sadata   / e\_TDW\_VEHICLE\_CATEGORY:GetModelStaticCategory | `modelid`                                                                                                                                                                                                                                                                                                                                                                                                                                       | -1 or category                   |
| vh\_sadata   / e\_TDW\_VEHICLE\_TYPE:GetModelStaticType         | `modelid`                                                                                                                                                                                                                                                                                                                                                                                                                                       | -1 or type                       |
| vh\_utils    / DestroyAllVehicles                               | `-`                                                                                                                                                                                                                                                                                                                                                                                                                                             | deleted vehicles                 |
| vh\_utils    / CountOfValidVehicles                             | `-`                                                                                                                                                                                                                                                                                                                                                                                                                                             | number of vehicles               |
| vh\_utils    / IsVehicleOccupied                                | `vehicleid`                                                                                                                                                                                                                                                                                                                                                                                                                                     | **true** or **false**            |
| vh\_utils    / IsVehicleSeatOccupied                            | `vehicleid, seatid`                                                                                                                                                                                                                                                                                                                                                                                                                             | **true** or **false**            |
| vh\_utils    / GetNearestVehicleFromPoint                       | `Float:x, Float:y, Float:z, Float:distance = 30.0`                                                                                                                                                                                                                                                                                                                                                                                              | vehicleid                        |
| vh\_utils    / GetVehicleOffsetFromPos                          | `vehicleid, Float:point_x, Float:point_y, Float:point_z, &Float:offset_x, &Float:offset_y, &Float:offset_z`                                                                                                                                                                                                                                                                                                                                     | -                                |
| vh\_utils    / GetVehicleBootPos                                | `vehicleid, &Float:x, &Float:y, &Float:z`                                                                                                                                                                                                                                                                                                                                                                                                       | **true** or **false**            |
| vh\_utils    / GetVehicleBonnetPos                              | `vehicleid, &Float:x, &Float:y, &Float:z`                                                                                                                                                                                                                                                                                                                                                                                                       | **true** or **false**            |
| vh\_utils    / GetVehicleRoofPos                                | `vehicleid, &Float:x, &Float:y, &Float:z`                                                                                                                                                                                                                                                                                                                                                                                                       | **true** or **false**            |
| vh\_utils    / GetVehicleMaxPassengers                          | `modelid`                                                                                                                                                                                                                                                                                                                                                                                                                                       | max passengers or 0b1111 (15)    |
| vh\_utils    / IsValidModelForPaintjob                          | `modelid`                                                                                                                                                                                                                                                                                                                                                                                                                                       | **true** or **false**            |
| vh\_utils    / GetVehicleDoorPos                                | `vehicletype, e_TDW_VEHICLE_DOOR:door, &Float:x, &Float:y, &Float:z`                                                                                                                                                                                                                                                                                                                                                                            | **true** or **false**            |
| vh\_utils    / GetVehicleWheelPos                               | `vehicletype, e_TDW_VEHICLE_WHEEL:wheel, &Float:x, &Float:y, &Float:z`                                                                                                                                                                                                                                                                                                                                                                          | **true** or **false**            |
| vh\_utils    / GetVehiclePanelsStatus                           | `vehicleid, &front_left_panel, &front_right_panel, &rear_left_panel, &rear_right_panel, &windshield, &front_bumper, &rear_bumper`                                                                                                                                                                                                                                                                                                               | **true** or **false**            |
| vh\_utils    / SetVehiclePanelsStatus                           | `vehicleid, front_left_panel, front_right_panel, rear_left_panel, rear_right_panel, windshield, front_bumper, rear_bumper`                                                                                                                                                                                                                                                                                                                      | **true** or **false**            |
| vh\_utils    / GetVehicleDoorsStatus                            | `vehicleid, &bonnet, &boot, &driver_door, &passenger_door`                                                                                                                                                                                                                                                                                                                                                                                      | **true** or **false**            |
| vh\_utils    / SetVehicleDoorsStatus                            | `vehicleid, bonnet, boot, driver_door, passenger_door`                                                                                                                                                                                                                                                                                                                                                                                          | **true** or **false**            |
| vh\_utils    / GetVehicleLightsStatus                           | `vehicleid, &light1, &light2, &light3, &light4`                                                                                                                                                                                                                                                                                                                                                                                                 | **true** or **false**            |
| vh\_utils    / SetVehicleLightsStatus                           | `vehicleid, light1, light2, light3, light4`                                                                                                                                                                                                                                                                                                                                                                                                     | **true** or **false**            |
| vh\_utils    / GetVehicleTiresStatus                            | `vehicleid, &tire1, &tire2, &tire3, &tire4`                                                                                                                                                                                                                                                                                                                                                                                                     | **true** or **false**            |
| vh\_utils    / SetVehicleTiresStatus                            | `vehicleid, tire1, tire2, tire3, tire4`                                                                                                                                                                                                                                                                                                                                                                                                         | **true** or **false**            |
| vh\_utils    / IsVehicleInWater                                 | `vehicleid`                                                                                                                                                                                                                                                                                                                                                                                                                                     | **true** or **false**            |
| vh\_utils    / IsVehicleInRangeOfPoint                          | `vehicleid, Float:range, Float:x, Float:y, Float:z`                                                                                                                                                                                                                                                                                                                                                                                             | **true** or **false**            |
| vh\_utils    / GetPlayerFromVehicleState                        | `vehicleid, stateid`                                                                                                                                                                                                                                                                                                                                                                                                                            | `INVALID_PLAYER_ID`  or playerid |
| vh\_utils    / GetPlayerFromVehicleSeat                         | `vehicleid, seatid`                                                                                                                                                                                                                                                                                                                                                                                                                             | `INVALID_PLAYER_ID`  or playerid |
| vh\_utils    / GetVehicleDriverId (_Macros_)                    | `vehicleid, seatid`                                                                                                                                                                                                                                                                                                                                                                                                                             | `INVALID_PLAYER_ID`  or playerid |
| vh\_utils    / SetVehicleWindowState (_SA:MP 0.3.7_)            | `vehicleid, e_TDW_VEHICLE_DOOR:door, e_TDW_WINDOW_STATE:newstate`                                                                                                                                                                                                                                                                                                                                                                               | **true** or **false**            |
| vh\_utils    / SetVehicleDoorState (_SA:MP 0.3.7_)              | `vehicleid, e_TDW_VEHICLE_DOOR:door, e_TDW_DOOR_STATE:newstate`                                                                                                                                                                                                                                                                                                                                                                                 | **true** or **false**            |
| vh\_utils    / GetVehicleWindowState (_SA:MP 0.3.7_)            | `vehicleid, door, w_states[e_TDW_VEHICLE_DOOR]`                                                                                                                                                                                                                                                                                                                                                                                                 | **true** or **false**            |
| vh\_utils    / GetVehicleDoorState (_SA:MP 0.3.7_)              | `vehicleid, door, w_states[e_TDW_VEHICLE_DOOR]`                                                                                                                                                                                                                                                                                                                                                                                                 | **true** or **false**            |
| vh\_utils    / Float:GetVehicleSpeedFromVelocity                | `Float:x, Float:y, Float:z, e_TDW_VEHICLE_SPEED:conv = kmph`                                                                                                                                                                                                                                                                                                                                                                                    | speed in float                   |
| vh\_utils    / Float:GetVehicleSpeed                            | `vehicleid, e_TDW_VEHICLE_SPEED:conv = kmph`                                                                                                                                                                                                                                                                                                                                                                                                    | speed in float                   |
| vh\_utils    / SetVehicleSpeed                                  | `vehicleid, Float:speed, e_TDW_VEHICLE_SPEED:conv = kmph`                                                                                                                                                                                                                                                                                                                                                                                       | -                                |
| vh\_utils    / OpenVehicleDoor (_Macros_)                       | `vehicleid, e_TDW_VEHICLE_DOOR:door`                                                                                                                                                                                                                                                                                                                                                                                                            | **true** or **false**            |
| vh\_utils    / CloseVehicleDoor (_Macros_)                      | `vehicleid, e_TDW_VEHICLE_DOOR:door`                                                                                                                                                                                                                                                                                                                                                                                                            | **true** or **false**            |
| vh\_utils    / IsVehicleDoorInState (_Macros_)                  | `vehicleid, e_TDW_VEHICLE_DOOR:door, e_TDW_DOOR_STATE:state`                                                                                                                                                                                                                                                                                                                                                                                    | **true** or **false**            |
| vh\_utils    / OpenVehicleWindow (_Macros_)                     | `vehicleid, e_TDW_VEHICLE_DOOR:door`                                                                                                                                                                                                                                                                                                                                                                                                            | **true** or **false**            |
| vh\_utils    / CloseVehicleWindow (_Macros_)                    | `vehicleid, e_TDW_VEHICLE_DOOR:door`                                                                                                                                                                                                                                                                                                                                                                                                            | **true** or **false**            |
| vh\_utils    / IsVehicleWindowInState (_Macros_)                | `vehicleid, e_TDW_VEHICLE_DOOR:door, e_TDW_WINDOW_STATE:state`                                                                                                                                                                                                                                                                                                                                                                                  | **true** or **false**            |
| vhs\_label   / CreateVehicle3DTextLabel                         | With Streamer: `vehicleid, const label[], color, Float:offset_x, Float:offset_y, Float:offset_z, Float:drawdistance, virtualworld, bool:testLos = false , interiorid = -1, Float:streamdistance = STREAMER_3D_TEXT_LABEL_SD, label_length = sizeof label` <br> Without: `vehicleid, const label[], color, Float:offset_x, Float:offset_y, Float:offset_z, Float:drawdistance, virtualworld, bool:testLos = false , label_length = sizeof label` | **true** or **false**            |
| vhs\_label   / DestroyVehicle3DTextLabel                        | `vehicleid`                                                                                                                                                                                                                                                                                                                                                                                                                                     | -                                |
| vhs\_label   / UpdateVehicle3DTextLabel                         | `vehicleid, const label[], bool:replace = true, color = -1`                                                                                                                                                                                                                                                                                                                                                                                     | **true** or **false**            |
| vhs\_label   / ShowVehicle3DTextLabel                           | `vehicleid`                                                                                                                                                                                                                                                                                                                                                                                                                                     | **true** or **false**            |
| vhs\_label   / HideVehicle3DTextLabel                           | `vehicleid`                                                                                                                                                                                                                                                                                                                                                                                                                                     | **true** or **false**            |
| vhs\_surfing / VehicleSurfing_Init                              | `playerid`                                                                                                                                                                                                                                                                                                                                                                                                                                      | -                                |
| vhs\_surfing / VehicleSurfing_Deinit                            | `playerid`                                                                                                                                                                                                                                                                                                                                                                                                                                      | -                                |
| vhs\_surfing / VehicleSurfing_SetAllowModel                     | `modelid, bool:value`                                                                                                                                                                                                                                                                                                                                                                                                                           | **true** or **false**            |

#### Constants list

| Constant                              | Value                                         | Note                 |
|---------------------------------------|:----------------------------------------------|----------------------|
| `VEHICLE_PAINTJOB_MIN`                | 0                                             |                      |
| `VEHICLE_PAINTJOB_MAX`                | 2                                             |                      |
| `INVALID_VEHICLE_ID`                  | 3                                             |                      |
| `MAX_INTERIORS`                       | 18                                            |                      |
| `MAX_VEHICLE_MODEL_ID`                | 611                                           |                      |
| `MIN_VEHICLE_MODEL_ID`                | 400                                           |                      |
| `MAX_VEHICLE_MODELS`                  | `MAX_VEHICLE_MODEL_ID - MIN_VEHICLE_MODEL_ID` |                      |
| `TDW_MAX_TIMER_INTERVAL` (_internal_) | 300                                           | for a surfing timer  |
| `TDW_MIN_SURF_SPEED`     (_internal_) | 20.0                                          | for a surfing timer  |
| `TDW_MAX_LABEL_SIZE`     (_internal_) | 256                                           | for labels           |

You can define special constants before `a_samp`.

#### The special constant list:

| Constant                               | Note                                            |
|----------------------------------------|-------------------------------------------------|
| TDW\_VEHICLE\_NOT\_USE\_FOREACH        | -                                               |
| TDW\_VEHICLE\_NOT\_USE\_STREAMER       | -                                               |
| TDW\_VEHICLE\_NOT\_USE\_SSCANF         | -                                               |
| \_TDW\_VEHICLE\_NOT\_USE\_PUBLICS      | If you don't want to use the functions(publics) |

#### New callbacks list:
````PAWN
OnVehicleWindowUpdate(vehicleid, e_TDW_VEHICLE_DOOR:door, e_TDW_WINDOW_STATE:newstate);
OnVehicleDoorUpdate(vehicleid, e_TDW_VEHICLE_DOOR:door, e_TDW_DOOR_STATE:newstate);
````