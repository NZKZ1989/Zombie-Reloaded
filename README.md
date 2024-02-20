ZombieReloaded
Infection/survival style gameplay for sourcemod

Commands
Public
buy - Buy a specific weapon
autobuy - AutoRebuy saved setup when spawning
rebuy - Rebuy saved setup
zshield - Deploy the shield, if available.
cds - Toggle infection countdown sound.
zmenu - Opens ZR's main menu.
zclass - Opens class selection menu.
scream - Emits a scream sound, if the player is a zombie.
moan - Emits a moan sound, if the player is a zombie.
zmarket - Opens custom buymenu.
zadmin - Opens ZR admin menu.
zcookies - Toggle all ZR cookies here.
zhp - Shows real HP as zombie.
zspawn - Spawn into the game after joining late.
ztele - Teleport back to spawn if you are stuck.
zr_antistick_dump_group - Dumps collision group data on one or more players. Usage zr_antistick_dump_group [#userid|name]
zr_log_list - List available logging flags and modules with their status values.
zr_log_add_module - Add one or more modules to the module filter. Usage: zr_log_add_module [module] ...
zr_log_remove_module - Remove one or more modules from the module filter. Usage: zr_log_remove_module [module] ...
zr_version - Prints version info about this plugin.
Admin
zr_infect - Infect a client. Usage: zr_infect [respawn - 1/0]
zr_human - Turn a client into a human. Usage: zr_human [respawn - 1/0]
zr_config_reload - Reloads a config file. Usage: zr_config_reload
zr_config_reloadall - Reloads all config files. Usage: zr_config_reloadall
zr_hitgroup - Toggles or sets if a zombie's hitgroup can be damaged. Usage: zr_hitgroup [1/0]
zr_hitgroup_enable_all - Enables all zombie hitgroups to be damaged. Usage: zr_hitgroup_enable_all
zr_hitgroup_headshots_only - Disables all zombie hitgroups but the head. Usage: zr_hitgroup_headshots_only
zr_class_dump - Dumps class data at a specified index in the specified cache. Usage: zr_class_dump <index|targetname>
zr_class_dump_multipliers - Dumps class attribute multipliers for the specified team. Usage: zr_class_dump_multipliers <"zombies"|"humans">
zr_class_modify - Modify class data on one or more classes. Usage: zr_class_modify <identifier|"zombies"|"humans"|"admins"> [is_multiplier]
zr_class_set_multiplier - Sets the multiplier on a class attribute. Usage: zr_class_set_multiplier <"zombies"|"humans">
zr_class_reload - Refreshes the player cache and reloads class attributes on one or more players. Usage: zr_class_reload
zr_vol_add - Creates a rectangular volume in the map. Usage: zr_vol_add [params]
zr_vol_remove - Removes an existing volume in the map. Usage: zr_vol_remove
zr_vol_list - Lists existing volumes in the map, or dumps detail data to the specified volume. Usage: zr_vol_list [volume index]
zr_vol_dumpstates - Dumps volume states for the specified player. Usage: zr_vol_dumpstates <index|targetname>
zr_restrict - Restricts a weapon or a weapon type. Usage: zr_restrict <weapon|weapon type> [weapon2|weapontype2] ...
zr_unrestrict - Unrestricts a weapon or a weapon type. Usage: zr_unrestrict <weapon|weapon type> [weapon2|weapontype2] ...
zr_zspawn_force - Force ZSpawn on a client. Usage: zr_zspawn_force ['0' = Spawn as human | '1' = Spawn as zombie]
zr_ztele_force - Force ZTele on a client. Usage: zr_ztele_force
Test
zrtest_is_valid_class_index - Returns whether the specified class index is valid or not. Usage: zrtest_is_valid_class_index
zrtest_get_active_class - Gets the current class the specified player is using. Usage: zrtest_get_active_class
zrtest_select_class - Selects a class for a player. Usage: zrtest_select_class
zrtest_get_class_by_name - Gets class index by class name. Usage: zrtest_get_class_by_name
zrtest_get_class_display_name - Gets class display name. Usage: zrtest_get_class_display_name
zrtest_iszombie - Returns whether a player is a zombie or not. Usage: zrtest_iszombie
zrtest_ishuman - Returns whether a player is a human or not. Usage: zrtest_ishuman
zrtest_infect - Infects a player. Usage: zrtest_infect
zrtest_human - Turns a player back into a human. Usage: zrtest_human
zrtest_push_player - Push a player. Usage: zrtest_push_player [0|1 - base velocity]
zrtest_parent - Prints your parent entity.
zrtest_friction - Prints your floor friction multiplier.
zrtest_maxspeed - Prints your max speed.
zrtest_killed_by_world - Gets or sets the killed by world value. Usage: zrtest_killed_by_world [1|0]
zrtest_respawn - Respawn a player. Usage: zrtest_respawn
zrtest_weaponslots - Lists weapon slots. Usage: zrtest_weaponslots [target]
zrtest_weaponlist - Lists all weapons. Usage: zrtest_weaponlist [target]
zrtest_knife - Gives a knife. Usage: zrtest_knife [target]
zrtest_removeweapons - Removes all weapons. Usage: zrtest_removeweapons [target]
Debug
zr_getparametercount - Test GetParameterCount function in paramtools.inc. Usage: zr_getparametercount
zr_getparametervalue - Test GetParameterValue function in paramtools.inc. Usage: zr_getparametervalue
Cvars
All
zr_log - 1 - "Enable logging of events in the plugin. Fatal errors are always logged.
zr_log_flags - "2 - "A bit field that specify what event types to log. See logging section (3.3) in manual for details.
zr_log_module_filter - "0 - "Enable module filtering. Only events from listed modules will be logged.
zr_log_ignore_console - "1 - "Don't log events triggered by console commands that are executed by the console itself, like commands in configs. Enable this command to avoid spamming logs with events like weapon restrictions.
zr_log_error_override - "1 - "Always log error messages no matter what logging flags or modules filters that are enabled.
zr_log_print_admins - "0 - "Print log events to admin chat in addition to the log file.
zr_log_print_chat - "0 - "Print log events to public chat in addition to the log file.
zr_config_path_models - "configs/zr/models.txt - "Path, relative to root sourcemod directory, to models config file.
zr_config_path_downloads - "configs/zr/downloads.txt - "Path, relative to root sourcemod directory, to downloads file.
zr_config_path_playerclasses - "configs/zr/playerclasses.txt - "Path, relative to root sourcemod directory, to playerclasses config file.
zr_config_path_weapons - "configs/zr/weapons.txt - "Path, relative to root sourcemod directory, to weapons config file.
zr_config_path_hitgroups - "configs/zr/hitgroups.txt - "Path, relative to root sourcemod directory, to hitgroups config file.
zr_permissions_use_groups - "0 - "Use group authentication instead of flags to access admin features. Generic admin flag is still required on some features.
zr_classes_menu_spawn - "0 - "Re-display class selection menu every spawn.
zr_classes_menu_join - "0 - "Display class selection menu when a player spawn for the first time.
zr_classes_random - "0 - "Player is assigned a random class every spawn. [Override: zr_classes_default_*]
zr_classes_change_timelimit - "20 - "Time limit to change human class with instant change after spawning. Time is in seconds. Use 0 or negative to disable.
zr_classes_save - 1 - "Save players' class selections in server cookies and restore when connecting. [Override: zr_classes_default_*]
zr_classes_default_zombie - "random - "Zombie class assigned to players on connect. ["random"
zr_classes_default_mother_zombie - "motherzombies","Zombie class assigned to mother zombies. ["motherzombies"
zr_classes_default_human - "random - "Human class assigned to players on connect. ["random"
zr_classes_default_admin - "default - "(Not implemented!) Admin-only class assigned to admins on connect, if any. ["default"
zr_classes_default_admin_mode - "random - "(Incomplete) Admin-mode class assigned to admins on connect. Do not confuse this with admin-only classes. ["random"
zr_classes_zombie_select - "1 - "Allow players to select zombie classes.
zr_classes_human_select - "1 - "Allow players to select human classes.
zr_classes_admin_select - "1 - "Allow admins to select admin mode classes. (Not to be confused by admin-only classes!)
zr_classes_speed_method - "prop - "Speed method to use when applying player speed. Do not touch this if you don't know what you're doing! ["lmv"
zr_classes_csgo_knockback_boost - "1 - "CS: GO only: Applies an upwards boost if necessary as a workaround for low knock back when standing on the ground. Side effects: Weaker and flying zombies (compensate with lower knock back).
zr_classes_menu_autoclose - "1 - "Automatically close class selection menu after selecting a class.
zr_classes_overlay_toggle - "1 - "Allow players to toggle class overlay.
zr_classes_overlay_togglecmds - "nightvision - "List of commands to hook that players can use to toggle class overlay. [Dependency: zr_classes_overlay_toggle | Delimiter: ","]
zr_classes_overlay_default - "1 - "Default class overlay toggle state set on connecting player.
zr_weapons - 1 - "Enable weapons module, disabling this will disable any weapons-related features. (weapon restrictions, weapon knockback multipliers, etc)
zr_weapons_restrict - "1 - "Enable weapon restriction module, disabling this will disable weapon restriction commands.
zr_weapons_restrict_endequip - "1 - "Restricts zombies from picking up weapons after the round has ended but before the next round has begun.
zr_weapons_zmarket - "1 - "Allow player to buy from a list of weapons in the weapons config.
zr_weapons_zmarket_buyzone - "1 - "Requires player to be inside a buyzone to use ZMarket. [Dependency: zr_weapons_zmarket]
zr_weapons_zmarket_norefill - "1 - "Dont allow users to rebuy weapons to refill their clip. [Dependency: zr_weapons_zmarket]
zr_weapons_zmarket_freespawn - "1 - "Purchases are free before the first zombie spawns. [Dependency: zr_weapons_zmarket]
zr_weapons_zmarket_rebuy - "1 - "Allow players to rebuy their previous weapons. [Dependency: zr_weapons_zmarket]
zr_weapons_zmarket_rebuy_auto - "1 - "Automatically equip default or loadout weapons. [Dependency: zr_weapons_zmarket&zr_weapons_zmarket_rebuy]
zr_weapons_zmarket_rebuy_primary","P90 - "Default primary weapon. [Dependency: zr_weapons_zmarket&zr_weapons_zmarket_rebuy]
zr_weapons_zmarket_rebuy_secondary","Elite - "Default secondary weapon. [Dependency: zr_weapons_zmarket&zr_weapons_zmarket_rebuy]
zr_hitgroups - "1 - "Enable hitgroups module, disabling this will disable hitgroup-related features. (hitgroup knockback multipliers, hitgroup damage control)
zr_infect_mzombie_mode - "dynamic - "Mother zombie infection mode. ['dynamic'
zr_infect_mzombie_ratio - "7 - "Dynamic mode: Infection ratio. Every n-th player is infected. | Absolute mode: Number of zombies to infect (positive ratio), or number of humans to keep (negative ratio).
zr_infect_mzombie_min - "1 - "Minimum number of mother zombies. Range mode only, cannot be zero.
zr_infect_mzombie_max - "3 - "Maximum number of mother zombies. Range mode only, cannot be zero.
zr_infect_mzombie_countdown - "0 - "Counts down to the first infection of the round. Countdown is printed in the middle of the client's screen.
zr_infect_mzombie_countdown_sound","0 - "Play back countdown sound to clients. [0
zr_infect_mzombie_respawn - "0 - "Teleport mother zombies back to spawn on infect.
zr_infect_spawntime_min - "30.0 - "Minimum time from the start of the round until picking the mother zombie(s).
zr_infect_spawntime_max - "50.0 - "Maximum time from the start of the round until picking the mother zombie(s).
zr_infect_consecutive_block - "1 - "Prevent a player from being chosen as mother zombie two rounds in a row.
zr_infect_round_robin - "1 - "Use randomized round-robin (with SteamID cache) for mother zombie infection.
zr_infect_round_robin_rtd - "1 - "Roll the dice for players new to the random round-robin SteamID cache to make it fair for late joiners.
zr_infect_weapons_drop - "1 - "Force player to drop all weapons on infect, disabling this will strip weapons instead.
zr_infect_knife_cooldown - "1.0 - "Time in seconds during which knife can not be used after becoming a zombie.
zr_infect_max_distance - "80.0 - "The maximum allowed distance between a client and an attacker for a successful infection. [0.0
zr_infect_teleport - "0 - "Teleports on infect to zombie.
zr_infect_explosion - "1 - "Disabling this will disable the fireball, smoke cloud, and sparks in a more efficient way.
zr_infect_fireball - "1 - "Spawn a fireball effect around player on infection. [Dependency: zr_infect_explosion]
zr_infect_smoke - "1 - "Spawn a smoke cloud effect around player on infection. [Dependency: zr_infect_explosion]
zr_infect_sparks - "1 - "Emit sparks from player on infection. [Dependency: zr_infect_explosion]
zr_infect_esplash - "1 - "Emit an energy splash from player on infection.
zr_infect_shake - "1 - "Shake player's view on infect.
zr_infect_shake_amp - "15.0 - "Amplitude of shaking effect. [Dependency: zr_infect_shake]
zr_infect_shake_frequency - "1.0 - "Frequency of shaking effect. [Dependency: zr_infect_shake]
zr_infect_shake_duration - "5.0 - "Duration of shaking effect. [Dependency: zr_infect_shake]
zr_damage_hitgroups - "1 - "Read hitgroup damage control from hitgroup config file, disabling this allows all zombie hitgroups to be shot.
zr_damage_block_ff - "1 - "Block friendly fire.
zr_damage_block_blast - "1 - "Block blast damage inflicted on self or teammates.
zr_damage_suicide_zombie - "0 - "Intercept suicide commands attempted by zombies.
zr_damage_suicide_mzombie - "1 - "Intercept suicide commands attempted by mother zombies.
zr_damage_suicide_human - "0 - "Intercept suicide commands attempted by humans.
zr_damage_suicide_cmds - "kill, spectate, jointeam, joinclass, explode - "List of client commands to intercept as suicide attempts. [Delimiter: \ - "]
zr_damage_suicide_after_infect - "1 - "Intercept suicide commands only after the first zombie has spawned.
zr_overlays_update_time - "1.0 - "How often to update overlays on players. [0.0
zr_overlays_min_dxlevel - "80 - "Minimum DirectX level allowed for overlays (mat_dxlevel).
zr_roundend_overlay - "1 - "Show specified overlay to players depending on winner when the round ends.
zr_roundend_overlays_human - "overlays/zr/humans_win - "Overlay, relative to "materials" folder, to display when humans win the round. [Dependency: zr_roundend_overlay]
zr_roundend_overlays_zombie - "overlays/zr/zombies_win - "Overlay, relative to "materials" folder, to display when zombies win the round. [Dependency: zr_roundend_overlay]
zr_roundend_balance_teams - "1 - "Balances the team every time the round ends. Disable this if you use something else to balance teams.
zr_roundend_zombies_win - "1 - "Should zombies win if roundtime runs out.
zr_account_cashfill - "1 - "Reset player's cash each spawn.
zr_account_cashfill_value - "12000 - "Amount of cash to set player's account to. [Dependency: zr_account_cashfill]
zr_account_cashdmg - "0 - "Attacker receives amount of cash equivalent to the damage that was inflicted.
zr_veffects_lightstyle - "0 - "Change lightstyle (brightness) of the map.
zr_veffects_lightstyle_value - "b - "Lightstyle value. ['a'
zr_veffects_sky - "0 - "Change map skybox.
zr_veffects_sky_path - "sky_borealis01up.vmt - Skybox file, relative to "materials/skybox" folder, to change map skybox to. This file is automatically downloaded to clients. [Dependency: zr_veffects_sky]
zr_veffects_sun_disable - "0 - "Disable sun rendering on map.
zr_veffects_fog - "0 - "(UNSUPPORTED) Enable fog rendering on the map.
zr_veffects_fog_override - "0 - "(UNSUPPORTED) If fog exists already on the map, then replace with new modified fog. [Dependency: zr_veffects_fog]
zr_veffects_fog_pcolor - "255 255 255 - "(UNSUPPORTED) Primary color of the fog. [Dependency: zr_veffects_fog]
zr_veffects_fog_scolor - "255 255 255 - "(UNSUPPORTED) Secondary color of the fog. [Dependency: zr_veffects_fog]
zr_veffects_fog_density - "0.8 - "(UNSUPPORTED) Density (thickness) of the fog. [Dependency: zr_veffects_fog]
zr_veffects_fog_startdist - "0 - "(UNSUPPORTED) Distance from player to start rendering foremost fog. [Dependency: zr_veffects_fog]
zr_veffects_fog_enddist - "400 - "(UNSUPPORTED) Distance from player to stop rendering fog. [Dependency: zr_veffects_fog]
zr_veffects_fog_farz - "2000 - "(UNSUPPORTED) Vertical clipping plane.
zr_veffects_ragdoll_remove - "1 - "Remove players' ragdolls from the game after a delay.
zr_veffects_ragdoll_dissolve - "-1 - "The ragdoll removal effect. ['-2'
zr_veffects_ragdoll_delay - "0.5 - "Time to wait before removing the ragdoll. [Dependency: zr_veffects_ragdoll_remove]
zr_voice - "0 - "(Incomplete) Modify sv_alltalk to obey zombie/human teams instead of t/ct.
zr_voice_zombies_mute - "0 - "(Incomplete) Only allow humans to communicate, block verbal zombie communication.
zr_seffects_moan - "30.0 - "Time between emission of a moan sound from a zombie.
zr_seffects_groan - "5 - "The probability that a groan sound will be emitted from a zombie when shot. ['100'
zr_seffects_death - "1 - "Emit a death sound when a zombie dies.
zr_seffects_command_limit - "4 - "Number of sound commands allowed within the time span, or total limit if time span is disabled. ['0'
zr_seffects_command_timespan - "10 - "Time span for sound command limiter (in seconds). ['0'
zr_ambientsounds - "1 - "Play an ambient sound to all players during gameplay.
zr_ambientsounds_file - "ambient/zr/zr_ambience.mp3 - "Sound file, relative to "sound" folder, to play as ambience. This file is automatically downloaded to clients. [Dependency: zr_ambientsounds]
zr_ambientsounds_length - "60.0 - "Length of the ambient sound. [Dependency: zr_ambientsounds]
zr_ambientsounds_volume - "0.8 - "Volume of the ambient sound. [1.0
zr_antistick - "1 - "Automatically unstick players when stuck within each others' collision hull.
zr_spawnprotect - "1 - "Player will be protected from infection when spawning into the game late.
zr_spawnprotect_time - "10 - "Amount of time to protect player. [Dependency: zr_spawnprotect]
zr_spawnprotect_speed - "250.0 - "Speed of the player during protection. See the manual for more information. [Dependency: zr_spawnprotect]
zr_spawnprotect_alpha - "0 - "Alpha of the player during protection. ['255'
zr_respawn - "0 - "Respawn players after death. [Recommended: (Enable) zr_zspawn*]
zr_respawn_delay - "1 - "Time after death to delay player respawn. [Dependency: zr_respawn]
zr_respawn_team_zombie - "1 - "Respawn player as a zombie. [Dependency: zr_respawn]
zr_respawn_team_zombie_world - "1 - "Respawn player as a zombie if player was a zombie and killed by world damage. [Override: zr_respawn_team_zombie]
zr_napalm_ignite - "1 - "Ignite grenade in mid-air after player throws it. [Dependency: Human Attribute 'has_napalm']
zr_napalm_time_reset - "1 - "The burn-time is reset when being naded multiple times. [0: Original burn-time is used.]
zr_napalm_time_scale - "75 - "The amount of damage that's needed to apply full burn duration.
zr_napalm_douse - "0 - "Minimum water-saturation before flame is extinguished. ['0'
zr_jumpboost_bhop_protect - "1 - "Prevent players from using forward jump boost multipliers to bunny hop.
zr_jumpboost_bhop_max - "300 - "The maximum horizontal velocity a player can achieve before bunnyhop protection kicks in. [Dependency: zr_jumpboost_bhop_protect]
zr_vol - "1 - "Enables volumetric features.
zr_vol_update_interval - "0.5 - "How often to update player positions and trigger events, in seconds.
zr_vol_trigger_interval - "0.5 - "How often to check for delayed events, in seconds. Use lower values for more precise delays.
zr_zspawn - "1 - "Allow players to spawn into the game late.
zr_zspawn_auto - "1 - "Should zspawn spawn joining players?
zr_zspawn_team_override - "1 - "Override spawn team when spawning by means of ZSpawn.
zr_zspawn_team_zombie - "0 - "Spawn player on zombie team when spawning by means of ZSpawn. [Dependency: zr_zspawn_team_override | Override: zr_respawn_team_zombie]
zr_zspawn_block_rejoin - "1 - "Block players disconnecting and rejoing the game using zspawn.
zr_zspawn_timelimit - "1 - "Put a time limit on the use of ZSpawn.
zr_zspawn_timelimit_time - "120.0 - "Time from the start of the round to allow ZSpawn. [Dependency: zr_zspawn_timelimit]
zr_zspawn_timelimit_zombie - "1 - "Spawn player on the zombie team AFTER the timelimit is up. ['-1'
zr_zhp - "1 - "Allow player to toggle real HP display as a zombie.
zr_zhp_default - "1 - "Default ZHP toggle state set on connecting player. [Dependency: zr_zhp]
zr_knockback_maxvel - 0 - Set maximum velocity zombies can get from knockback ['0'
zr_ztele_zombie - "1 - "Allow zombies to use ZTele.
zr_ztele_human_before - "1 - "Allow humans to use ZTele before the mother zombie has spawned.
zr_ztele_human_after - "1 - "Allow humans to use ZTele after the mother zombie has spawned.
zr_ztele_delay_zombie - "3.0 - "Time between using ZTele command and teleportation for zombies. [Dependency: zr_ztele_zombie]
zr_ztele_delay_human - "3.0 - "Time between using ZTele command and teleportation for humans. [Dependency: zr_ztele_human_(before)/(after)]
zr_ztele_max_zombie - "3 - "Max number of times a zombie is allowed to use ZTele per round. [Dependency: zr_ztele_zombie]
zr_ztele_max_human - "1 - "Max number of times a human is allowed to use ZTele per round. [Dependency: zr_ztele_human_(before)/(after)]
zr_ztele_autocancel - "1 - "Automatically cancel ZTele if player moves out of a set boundary. [Dependency: zr_ztele_(zombie)/(human)[_(before)/(after)]]
zr_ztele_autocancel_distance - "20 - "Maximum distance, in feet, player is allowed to travel before teleport is cancelled. [Dependency: zr_ztele_autocancel]
zr_ztele_random_spawn - "0 - "Teleport player to a random spawn point instead of the players initial one, when using ztele.
