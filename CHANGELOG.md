# Changelog v1.3.3

- Added `setScanForATMs` export to support upcoming integration with the FS-Robberies script.

# Changelog v1.3.2

- Added a new `getMoney` export for client-side use.
- You can now toggle individual elements in the built-in Money HUD through the config. This is useful if you’re using a custom HUD that already displays cash, bank, or dirty money, but you still want the built-in HUD to show elements like “pokerchips.”

# Changelog v1.3.1

- Major performance improvements, reduced resmon usage from 0.90–1.00ms to 0.06–0.15ms (tested on a good system).
- Improved ATM walk-up logic for much more accurate positioning.
- Added new config option to hide text prompts.

# Changelog v1.3.0

- Added support for customizing the bank name displayed on ATMs.
- Added `/paytap` to let players pay using their phone when the receiving player provides a pay terminal (via Mrs. Bzzz).
- Renamed `/setplayerdirty` to `/setplayerdirtymoney` for better clarity.
- Added `/paydirtymoney` to allow paying someone dirty cash directly.
- Added a generic "pay" option that removes money from the player without sending it to anyone, useful for RP scenarios.
- Added `/togglemoneyhudtheme` to let players change their money HUD theme anywhere (can still be changed at ATMs too).
- Added optional debug logs for the database auto-update process; enable them with `Config.debug = true` to see detailed startup actions if updates fail.
- Fixed an issue where the automatic database updater sometimes failed to apply changes, which could result in server errors.

# Changelog v1.2.0

- Added admin commands to set player balances by server ID: /setplayercash, /setplayerbank, /setplayerdirty, /setplayerpokerchips
- Added a new HUD element that shows the amount added or removed when money changes
- Fixed UI bug where long decimals like 500.349999999954543 now round properly to values like 500.49

# Changelog v1.1.1

- Added a new parameter to the `addMoney` and `removeMoney` exports to control whether a notification is shown to the player.

# Changelog v1.1.0

— Introduced **Poker Chips** as a new currency type  
— Poker Chips are automatically added to your database if already initialized, so you don’t need to update your SQL manually  
— Added a built-in Money HUD (can be disabled if using a custom HUD)  
— Added `/paychips` command to transfer poker chips to another player  
— Fixed an issue where attempting to pay cash to an invalid player ID would cause a server error (now safely does nothing)  
— Cleaned up old and unused code for better performance
