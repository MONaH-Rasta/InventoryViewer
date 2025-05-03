# Inventory Viewer

Oxide plugin for Rust. Look into a player's inventory.

Allows players to check and loot another player's inventory.

## Permissions

* `inventoryviewer.allowed` -- Required to use inventory viewer.
* `inventoryviewer.unlock` -- Required to be able to give and take items from an inventory you are viewing.

## Commands

This plugin provides universal chat and console commands. When using a command in the chat, prefix it with a forward slash: `/`.

* `viewinv`, `viewinventory`, `inspect` -- view the inventory of a player you are looking at. Add a space and a steamid or player name to select players individually.

*If you just wish to use the raycast feature to view the inventory of a player you are looking at a key bind may be set up using `bind key viewinv ""`.*

## Backpacks

Right click a backpack when viewing a player to view the backpacks contents. Then the escape button to return to the original player inventory view.

## Configuration

```json
{
  "View inventory raycast distance": 10.0,
  "View inventory timeout (seconds) set to 0 to disable": 60.0,
  "Use console logging": false,
  "Use discord logging": false,
  "Webhook URL": "",
  "Discord name": "Inventory Viewer",
  "Discord avatar URL": "https://i.imgur.com/BLoVcpz.png"
}
```

## For Developers

### API

```csharp
void _ViewInventory(BasePlayer player, BasePlayer targetplayer)
```

## Credits

* **Mughisi**, the previous author of this plugin
