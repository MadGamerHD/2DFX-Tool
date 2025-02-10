RELEASE INFO   
   2DFX TOOL FOR GTA: SAN ANDREAS
   AUTHOR: DK22PAC
   VERSION: 03.03.2015

DESCRIPTION
   THIS TOOL GENERATES 2DFX DATA FOR DFF MODELS

DOCUMENTATION
   USING FLAGS
      TO COMBINE 2 OR MORE FLAGS, YOU JUST NEED TO PUT COMMA SYMBOL (,) BETWEEN THEM. FOR EXAMPLE,
         Flags1 AT_DAY,AT_NIGHT
      TO SKIP ALL FLAGS, USE (-) SYMBOL. FOR EXAMPLE,
         Flags2 -

   EFFECT TYPES (BOTH V1 AND V2 ARE USABLE)
      V1               V2            DESCRIPTION
      LIGHT                          Attaches a light to object
      PARTICLE                       Attaches particle effect to object
      PED              PED_ATTRACTOR Attracts ped to object
      SUNFLARE         SUNGLARE      Attaches sun glare effect to object
      ENEX                           Attaches an enter-exip teleport to object
      ROADSIGN                       Attaches road sign text to object
      SLOTMACHINEWHEEL               Defines slot machine wheel object in casino
      NAVIPOINT        COVERPOINT    A place where peds could cover while acting in firefight
      ESCALATOR                      Attaches an escalator stairs to object
   !TYPE (EXPLOSION) IS NOT USED IN SAN ANDREAS, TYPE (FURNITUR) CAN BE DEFINED ONLY WITHIN .IDE 2DFX SECTION

   CORONA MODE (BOTH V1 AND V2 ARE USABLE, USING NUMBERS (0-13) INSTEAD OF NAME IS ALSO POSSIBLE)
      #  V1                    V2                                   DESCRIPTION
      0  DEFAULT                                                    No special behaviour for corona
      1                        RANDOM_FLASHING                      Random flashing
      2  ALWAYS_AT_WET_WEATHER RANDOM_FLASHIN_ALWAYS_AT_WET_WEATHER Random flashing (only if weather is not "wet")
      3                        LIGHTS_ANIM_SPEED_4X                 Lights will flash successively (speed = 4x)
      4                        LIGHTS_ANIM_SPEED_2X                 Lights will flash successively (speed = 2x)
      5                        LIGHTS_ANIM_SPEED_1X                 Lights will flash successively (speed = 1x)
      7  TRAFFICLIGHT                                               Defines a trafficlight behaviour
      8  TRAINCROSSLIGHT                                            Defines a train crosslight behaviour
      10 AT_RAIN_ONLY                                               Corona is shown only at rainy weather
      11                       5S_ON_5S_OFF                         5s - enabled, 5s - disabled (seconds)
      12                       6S_ON_4S_OFF                         6s - enabled, 4s - disabled
      13                       6S_ON_4S_OFF_2                       6s - enabled, 4s - disabled
   !TYPE 6 IS UNKNOWN, TYPE 9 IS NOT VALID
   
   LIGHT FLAGS 1
      NAME                         DESCRIPTION
      CORONA_CHECK_OBSTACLES       Don't draw corona if there are obstacles between camera and corona
      FOG_TYPE1                    Defines type of fog effect that is visible under light
      FOG_TYPE2                    Defines type of fog effect that is visible under light
      WITHOUT_CORONA               Don't draw corona
      CORONA_ONLY_AT_LONG_DISTANCE Corona is visible only from long distance
      AT_DAY                       Light is enabled at day time
      AT_NIGHT                     Light is enabled at night time
      BLINKING1                    Light blinking, type 1

   LIGHT FLAGS 2
      NAME                         DESCRIPTION
      CORONA_ONLY_FROM_BELOW       Corona is visible only if camera is placed under corona
      BLINKING2                    Light blinking, type 2
      UDPDATE_HEIGHT_ABOVE_GROUND  
      CHECK_DIRECTION              Draw corona only if camera is placed in some specific position (defined with "ViewVector" values)
      BLINKING3                    Light blinking, type 3

   PED ATTRACTOR TYPES (BOTH V1 AND V2 ARE USABLE, USING NUMBERS (0-9) INSTEAD OF NAME IS ALSO POSSIBLE)
      # V1                             V2                           DESCRIPTION
      0 USE_ATM_DAY_ONLY               PED_ATM_ATTRACTOR            Ped uses ATM (at day time only)
      1 SEAT_ON_BENCH_DAY_ONLY         PED_SEAT_ATTRACTOR           Ped seats (at day time only)
      2 STANDSTILL_DAY_ONLY            PED_STOP_ATTRACTOR           Ped stops (at day time only)
      3 STANDSTILL_THEN_GO_AWAY        PED_PIZZA_ATTRACTOR          Ped stops for few seconds
      4 GO_AWAY_BUT_STAY_IF_RAINY      PED_SHELTER_ATTRACTOR        Ped goes away after spawning, but stops if weather is rainy
      5 SCRIPTED                       PED_TRIGGER_SCRIPT_ATTRACTOR Launches a script ("ExternalScript" field must be filled with script name)
      6 STANDSTILL_GO_AWAY_2           PED_LOOK_AT_ATTRACTOR        Ped looks at object, then goes away
      7                                PED_SCRIPTED_ATTRACTOR       This type is not valid
      8 LIE_DAY_ONLY_GO_AWAY_AFTER_6PM PED_PARK_ATTRACTOR           Ped lies (at day time only, ped goes away after 6 PM)
      9 SEAT_AT_HOUSE                  PED_STEP_ATTRACTOR           Ped seats on steps
   !DO NOT MISS TYPE "SCRIPTED" WITH TYPE "PED_SCRIPTED_ATTRACTOR". THEY ARE DIFFERENT TYPES.
   !TYPE "PED_SCRIPTED_ATTRACTOR" IS NOT VALID

   ENEX FLAGS 1
      UNKNOWN_INTERIOR
      UNKNOWN_PAIRING
      CREATE_LINKED_PAIR
      REWARD_INTERIOR
      USED_REWARD_ENTRANCE
      CARS_AND_AIRCRAFT
      BIKES_AND_MOTORCYCLES
      DISABLE_ON_FOOT

   ENEX FLAGS 2
      ACCEPT_NPC_GROUP
      FOOD_DATE_FLAG
      UNKNOWN_BURGLARY
      DISABLE_EXIT
      BURGLARY_ACCESS
      ENTERED_WITHOUT_EXIT
      ENABLE_ACCESS
      DELETE_ENEX

   ROADSIGN COLORS
      WHITE
      BLACK
      GREEN
      RED

   ESCALATOR DIRECTION
      UP
      DOWN

SEE MORE INFO HERE:
http://gtaforums.com/topic/576214-tutsa-creating-2dfx-for-your-models/