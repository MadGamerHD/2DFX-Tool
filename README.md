## 2DFX-Tool

**Release Info:**  
**Tool for GTA: San Andreas**  
**Author:** DK22PAC  
**Version:** 03.03.2015

### Description  
The **2DFX Tool** is designed to generate 2DFX data for DFF models in *Grand Theft Auto: San Andreas*. It enables you to apply various flags, effect types, and behaviors to enhance your models in the game world.

---

### Documentation

#### **Using Flags**  
- To combine multiple flags, simply separate them with a comma.  
  Example: `Flags1 AT_DAY,AT_NIGHT`  
- To skip all flags, use the `-` symbol.  
  Example: `Flags2 -`

#### **Effect Types**  
The following effect types can be used (both V1 and V2 are supported):

| **V1** | **V2** | **Description** |
| ------ | ------ | --------------- |
| LIGHT  |        | Attaches a light to an object. |
| PARTICLE |      | Attaches a particle effect to an object. |
| PED    | PED_ATTRACTOR | Attracts a ped to an object. |
| SUNFLARE | SUNGLARE | Attaches a sun glare effect to an object. |
| ENEX   |        | Attaches an enter-exit teleport to an object. |
| ROADSIGN |      | Attaches road sign text to an object. |
| SLOTMACHINEWHEEL | | Defines a slot machine wheel object in a casino. |
| NAVIPOINT | COVERPOINT | A place where peds could cover while acting in a firefight. |
| ESCALATOR |       | Attaches an escalator to an object. |

Note: `EXPLOSION` is not used in GTA: San Andreas. The `FURNITUR` type can only be defined within the `.IDE 2DFX` section.

#### **Corona Modes**  
Corona modes (V1 and V2) can be used, and numerical values (0-13) can replace their names.

| **V1** | **V2** | **Description** |
| ------ | ------ | --------------- |
| 0      |        | No special behavior for the corona. |
| 1      | RANDOM_FLASHING | Random flashing. |
| 2      | ALWAYS_AT_WET_WEATHER | Random flashing, only in non-wet weather. |
| 3      | LIGHTS_ANIM_SPEED_4X | Lights flash at 4x speed. |
| 4      | LIGHTS_ANIM_SPEED_2X | Lights flash at 2x speed. |
| 5      | LIGHTS_ANIM_SPEED_1X | Lights flash at 1x speed. |
| 7      | TRAFFICLIGHT | Defines traffic light behavior. |
| 8      | TRAINCROSSLIGHT | Defines train crossing light behavior. |
| 10     | AT_RAIN_ONLY | Corona appears only during rain. |
| 11     | 5S_ON_5S_OFF | 5 seconds on, 5 seconds off. |
| 12     | 6S_ON_4S_OFF | 6 seconds on, 4 seconds off. |
| 13     | 6S_ON_4S_OFF_2 | 6 seconds on, 4 seconds off (another variant). |

Note: Type 6 is unknown, and Type 9 is not valid.

#### **Light Flags 1**  
| **Name**                         | **Description** |
| --------------------------------- | --------------- |
| CORONA_CHECK_OBSTACLES            | Prevents the corona from being drawn if there are obstacles between the camera and the corona. |
| FOG_TYPE1                         | Defines the type of fog effect visible under light. |
| FOG_TYPE2                         | Defines another type of fog effect visible under light. |
| WITHOUT_CORONA                    | Disables the corona. |
| CORONA_ONLY_AT_LONG_DISTANCE     | The corona is visible only from long distances. |
| AT_DAY                            | Light is enabled during the day. |
| AT_NIGHT                          | Light is enabled during the night. |
| BLINKING1                         | Light blinking type 1. |

#### **Light Flags 2**  
| **Name**                         | **Description** |
| --------------------------------- | --------------- |
| CORONA_ONLY_FROM_BELOW           | The corona is visible only when the camera is placed below it. |
| BLINKING2                         | Light blinking type 2. |
| UPDATE_HEIGHT_ABOVE_GROUND       | |
| CHECK_DIRECTION                   | Draw the corona only if the camera is positioned at a specific direction (defined with `ViewVector`). |
| BLINKING3                         | Light blinking type 3. |

#### **Ped Attractor Types**  
| **V1**                             | **V2**                           | **Description** |
| ----------------------------------- | --------------------------------- | --------------- |
| 0                                   | USE_ATM_DAY_ONLY                 | Ped uses ATM only during the day. |
| 1                                   | SEAT_ON_BENCH_DAY_ONLY           | Ped sits on a bench only during the day. |
| 2                                   | STANDSTILL_DAY_ONLY              | Ped stands still during the day. |
| 3                                   | STANDSTILL_THEN_GO_AWAY          | Ped stops for a few seconds, then goes away. |
| 4                                   | GO_AWAY_BUT_STAY_IF_RAINY        | Ped goes away after spawning, but stops if the weather is rainy. |
| 5                                   | SCRIPTED                         | Launches a script (external script must be specified). |
| 6                                   | STANDSTILL_GO_AWAY_2             | Ped stops, then goes away. |
| 8                                   | LIE_DAY_ONLY_GO_AWAY_AFTER_6PM   | Ped lies, goes away after 6 PM. |
| 9                                   | SEAT_AT_HOUSE                    | Ped seats on steps. |

#### **Enex Flags 1**
- UNKNOWN_INTERIOR  
- UNKNOWN_PAIRING  
- CREATE_LINKED_PAIR  
- REWARD_INTERIOR  
- USED_REWARD_ENTRANCE  
- CARS_AND_AIRCRAFT  
- BIKES_AND_MOTORCYCLES  
- DISABLE_ON_FOOT  

#### **Enex Flags 2**
- ACCEPT_NPC_GROUP  
- FOOD_DATE_FLAG  
- UNKNOWN_BURGLARY  
- DISABLE_EXIT  
- BURGLARY_ACCESS  
- ENTERED_WITHOUT_EXIT  
- ENABLE_ACCESS  
- DELETE_ENEX  

#### **Road Sign Colors**
- WHITE  
- BLACK  
- GREEN  
- RED  

#### **Escalator Direction**
- UP  
- DOWN  

For more details, visit the [official documentation](http://gtaforums.com/topic/576214-tutsa-creating-2dfx-for-your-models/).
