This plugin fixes players respawning wounded / incapacitated.

This bug happens when a player is flagged as "Incapacited" but not as "Wounded", which isn't supposed to happen. We aren't sure how exactly this is happening in the first place, but this plugin fixes the issue by automatically toggling off the "Incapacitated" flag for players when they spawn, if they are not flagged as "Wounded". Upon loading the plugin, any players already in the invalid state should be fixed as well.
