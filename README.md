This plugin is a temporary fix for players respawning wounded / incapacitated, until you can update Oxide.

## Do I need this plugin?

First, run `o.version` in your server console to determine your Oxide version.

If you are running Oxide v2.0.5105 or newer, you don't need this plugin, and you can stop reading now.

If you are running Oxide v2.0.5081 or older, and you are seeing players respawning in a wounded state, you should install this plugin. Update Oxide at your earliest convenience, and then uninstall this plugin. Note that if you simply update Oxide without installing this plugin, some players may still be stuck in wounded state until they are killed.

## What caused this bug?

The first Oxide release in July introduced a bug where players who became "Incapacitated" (wounded and unable to move) and then died, would stay Incapacitated every time they respawned. Oxide update v2.0.5081 fixed the root cause. However, players who already got stuck Incapacitated previously would stay that way, even after rebooting the server with the fix. To address this, Oxide v2.0.5105 introduced a change that would automatically fix players who had gotten stuck Incapacitated whenever they respawned next. While that fix was under way, this plugin was released to hotfix any servers that had not yet updated Oxide.
