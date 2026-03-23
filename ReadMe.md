Unfortunately I no longer play and haven't for years so am unable to fix issues or update. I will leave the code here public incase anyone wishes to take over 

# Lazy

Simple helper for farming XP/CP/Trash items. So far includes:

  - Always Turn to face Target, even if Trust Tank pulls away from you
  - Keep within 3Yalms of Target at all times
  - Weaponskill when TP available
  - Ability to cast a spell whenever Recast/MP allows
  - _SIMPLE_ auto target system

### Installation

* Inside your Windower\Addons folder create a new folder called Lazy
* Copy these files into the folder created above.

### Commands
* //lazy reload
* //lazy save
* //lazy show
* //lazy spell
* //lazy set_spell \<spell name\>
* //lazy ws
* //lazy set_ws \<weaponskill name\>
* //lazy autotarget
* //lazy set_target \<monster name\>
* //lazy clear_target
* //lazy pull
* //lazy ra
* //lazy jiggle \<key\>
* //lazy jiggle_interval \<seconds\>
* //lazy timer \<minutes\>

#### //lazy reload
Reloads the options from the settings.xml

#### //lazy save
Saves current settings to settings.xml for the logged-in character

#### //lazy show
Displays current settings and state

#### //lazy spell
Toggles spell casting on/off

#### //lazy set_spell \<spell name\>
Sets the spell to cast (e.g. `//lazy set_spell "Dia III"`)

#### //lazy ws
Toggles weaponskill use on/off

#### //lazy set_ws \<weaponskill name\>
Sets the weaponskill to use (e.g. `//lazy set_ws "Sanguine Blade"`)

#### //lazy autotarget
Toggles automatic target hunting on/off

#### //lazy set_target \<monster name\>
Sets/Changes the current auto target monster name

#### //lazy clear_target
Clears the auto target monster name

#### //lazy pull
Toggles pull mode on/off

#### //lazy ra
Toggles ranged attack mode on/off

#### //lazy jiggle \<key\>
Enables jiggle mode, pressing the given key periodically to prevent AFK logout (e.g. `//lazy jiggle numpad0`)

#### //lazy jiggle_interval \<seconds\>
Sets how often jiggle fires in seconds (minimum 5, default 60)

#### //lazy timer \<minutes\>
Runs Lazy for the specified number of minutes then stops automatically. Uses a timestamp set at the time of the command, checked on every engine tick. Call with no argument to cancel an active timer.

### settings.xml
```xml
<spell></spell>
<spell_active></spell_active>
<weaponskill></weaponskill>
<weaponskill_active></weaponskill_active>
<autotarget>false</autotarget>
<target>Monster Name<target>
```
* spell - Spell to cast, will cast whenever MP and recast time allows
* spell_active - true/false enables/disables enables casting of the spell
* weaponskill - weaponskill to use when over 1000TP
* weaponskill_active - true/false enables/disables use of weaponskills
* autotarget - true/false enables/disables automatic hunting of mobs in range
* target - name of monster to hunt
