# terraria-info
Informational files for the game Terraria.  Providing both CSV and JSON format for the use in APIs.  

Some of this information comes from the Terraria Crafting Recipes spreadsheet I found on Google docs.  I could not, however, find information about the author.  Some of the other information comes from the [Official Terraria Wiki](http://terraria.gamepedia.com).

Information on the Wiki and in the spreadsheet is licensed under CC BY-NC-SA 3.0.  This data is under the same licensing.

# Data Organization
Currently I have all of the data in a Google Sheets workbook with references.  The Recipes tab has both the item and ingredient names, along with their ID.  For exportation I don't export the name, but I keep it around because I use formulas to lookup the IDs.  Are IDs more useful, or are item names more useful?  In a relational database system, I believe that lookup IDs can be very useful especialy if item names ever change.  However, I do see how there could be some overhead.

# TODOS
* Add script for building JSON from CSV files.
* Figure out how to handle the Mobile/Console and PC differences.  Some items have IDs that are greater than 5000 and those are specific to certain platforms.  Crafting recipes might be different, so there are multiple recipe associations per item.

# Future Plans
I plan on implementing an API service for this information to help the Terraria community in creating bots, apps, and other services requiring the data.

# Pull Requests
Please submit a pull request with updates to the CSV files.  Once they are accepted, a process will convert them to JSON automatically.
