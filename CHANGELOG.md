# Changelog v1.1.1
- Added a new parameter to the `addMoney` and `removeMoney` exports to control whether a notification is shown to the player.

# Changelog v1.1.0
— Introduced **Poker Chips** as a new currency type  
— Poker Chips are automatically added to your database if already initialized, so you don’t need to update your SQL manually  
— Added a built-in Money HUD (can be disabled if using a custom HUD)  
— Added `/paychips` command to transfer poker chips to another player  
— Fixed an issue where attempting to pay cash to an invalid player ID would cause a server error (now safely does nothing)  
— Cleaned up old and unused code for better performance
