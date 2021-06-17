The functionality of the ATonSYSSTART MIDlet has been extended with a function allowing to change the setting of the AT+CEMODE command to 0.

This was accomplished by locating in NV memory, the bytes responsible for storing information about the current configuration of the AT+CEMODE command, and manually swapping these bytes so that their state represents the 0 setting.

In order to use this feature, the ATonSYSSTART MIDlet and its configuration file ATonSYSSTART.cfg must be placed in the module memory.
Then install it with the command AT^SJAM=0,"a:/ATonSYSSTART.jad",""
After module restart MIDlet should start automatically and change configuration from Voice Centric to Data Centric.