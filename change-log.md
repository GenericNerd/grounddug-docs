# Change Log

## GroundDug Alpha Rewrite 20y03w-01

### Added

* `g!badges` to display the level given by the bot to users. Check [documentation ](documentation/bot-commands-list.md)on usage.

### Changed

* Whole bot code base
  * Includes custom checks which links directly to level system
  * Includes custom GD permissions check instead of checking when command is ran \(derived from discord.Cog class\)
  * Rewrote embed generation to include async empty field value generation
  * System to allow all modules and cogs to be reloaded, including the core and developer modules. \(`Accessible only through Level 4 and above`\)
* Administrators of the server also now get the `GD_ADMINISTRATOR` permission when the bot joins the server.

## GroundDug Alpha 20y02w-07

### Added

* Level system to display developers and trusted users
* `g!kick` command

### Changed

* Logging method change for cogs

### 

## GroundDug Alpha 20y02w-06

### Added

* Asynchronous database handler.
  * Should stop the bot from going offline whenever it is added to guilds with over 100 members

### Removed

* Developer restart command to accommodate core module reload

### Changed

* Miscellaneous commands have been moved to their own seperate cog \(core\_cog.py\) to facilitate reloading.
  * This will reduce the need for restarts and planned downtime.

