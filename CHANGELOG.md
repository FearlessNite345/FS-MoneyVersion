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
