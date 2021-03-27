/*	-WHAT IS THIS?-
	This file adds optional material to "MPMB's Character Record Sheet" found at https://flapkan.com/mpmb/charsheets
	Import this file using the "Add Extra Materials" bookmark.

	-KEEP IN MIND-
	It is recommended to enter the code in a fresh sheet before adding any other information (i.e. before making your character with it).
*/

/*	-INFORMATION-
	Subject:	Race
	Effect:		This script adds a player race, called "Hexblood"
	Code by:	W2W
	Date:		2021 Mar 26

*/

var iFileName = "Hexblood.js";
RequiredSheetVersion(12.999);

SourceList["FRA:SS"] = {
	name : "Forgotten Realms Archetypes: Savagery & Shadow (v1.2)",
	abbreviation : "FRA:SS",
	group : "Dungeon Masters Guild",
	url : "https://www.dmsguild.com/product/208791/",
	date : "2017/04/14"
};

RaceList["Hexblood"] = {
	regExpSearch : /^(?=.*hex)(?=.*blood).*$/i,
	name : "Hexblood",
	sortname : "Hexblood",
	source : ["FRA:SS", 14],
	plural : "Hexblood ",
	size : 3,
	speed : { walk : { spd : 30, enc : 20 } },
	languageProfs : ["Common", 1],
	vision : [["Darkvision", 60]],
	dmgres : ["Charmed"],
	improvements : "Hexblood: +2 Any, +1 Any;",
	scores : [0, 0, 0, 0, 0, 0],
	trait : "Hexblood (+2 any, +1 any)\nmagic token: As an action, you can harmlessly pull out one of your nails, a tooth, or a lock of hair. This token is imbued with magic until you finish a long rest. While the token is imbued in this way, you can use an action to send a telepathic message to the creature holding or carrying the token, as long as you are on the same plane of existence and are within 10 miles of it. The message can contain up to twenty-five words.

In addition, while you are within 10 miles of the token, you can use an action to enter a trance for 1 minute, during which you can see and hear from the token as if you were located where it is. While you are using your senses at the token’s location, you are blinded and deafened in regard to your own surroundings. Afterward, the token is harmlessly destroyed.

Once you create a token using this feature, you can’t do so again until you finish a long rest, at which point your missing part regrows." + (typePF ? "\n" : " ") + "Hex Magic: You can cast the disguise self and hex spells with this trait. Intelligence, Wisdom, or Charisma is your spellcasting ability for these spells (choose when you gain this lineage). Once you cast either of these spells with this trait, you can’t cast that spell with it again until you finish a long rest. You can also cast these spells using any spells slots you have..\nDisguise Self: I can cast Disguise self." + (typePF ? "\n" : " ") + "Hex: I have the Hex cantrip.",
	spellcastingAbility : 6,
	spellcastingBonus : {
		name : "Hex Magic",
		spells : ["Hex Magic"],
		selection : ["Hex Magic"],
		atwill : true
	},
	features : {
		"Disguise Self" : {
			name : "Disguise Self",
			minlevel : 1,
			usages : 1,
			recovery : "long rest",
			action : ["bonus action", ""]
		},
		"Hex" : {
			name : "Hex",
			minlevel : 1,
			action : ["bonus action"]
		}
	}
};
