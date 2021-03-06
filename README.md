Various small scripts for working with exported data or API data from
HabitRPG ( http://habitrpg.com/  http://habitrpg.wikia.com/ ).

--------------------------------------------

habitrpg_user_data_display.html

A stand-alone JavaScript-enabled web page that reads a user's data and
displays such things as an unallocated points reminder, limited habit
history, quest progress, equipment lost from death, number of drops
received today, tasks that have not been tagged, etc.

More features added upon request (if possible and if time permits).

--------------------------------------------

habitrpg_content_parser.pl

This script parses the JSON data that describe's HabitRPG's "content"
(equipment, etc). It produces output depending on the command-line
parameter(s). For example:

	habitrpg_content_parser.pl listgearkeys
		lists the "key" and name for each piece of equipment:
			armor_base_0 :: Plain Clothing
			armor_healer_1 :: Acolyte Robe
			armor_healer_2 :: Medic Robe
			....
			weapon_wizard_4 :: Brass Staff
			weapon_wizard_5 :: Archmage Staff
			weapon_wizard_6 :: Golden Staff

	habitrpg_content_parser.pl infobox weapon_wizard_4
		Creates a basic infobox for adding to the wiki.
		Specify either the key for one piece of equipment or
		"all" to create infoboxes for all of them.

			{{infobox item
			| title         = Brass Staff
			| image         = Brassstaff.png
			| imagecaption  = As powerful as it is heavy. Increases INT by 12 and PER by 5.
			| buy           = 120g
			| sell          = N/A
			| bonus         = +12 to INT; +5 to PER
			}}


Slightly more information here:
	http://habitrpg.wikia.com/wiki/Thread:9471

Comments, suggestions, and pull requests welcome.

--------------------------------------------

Contact:

	Alys (Alice Harris)
	http://habitrpg.wikia.com/wiki/User:LadyAlys
	lady_alys@oldgods.net
