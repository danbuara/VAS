Hello! Thank you for using my Virtual Ammobox System (VAS). This was created for a specific mission to cut back on network lag & ammo box usage and well decided to release for public!

System is very easy to use, to add this to your mission copy the gear folder from the scripts folder to your mission folder, edit description.ext and put:

#include "VAS\menu.hpp"

class CfgFunctions
{
	#include "VAS\cfgfunctions.hpp"
};

Somewhere in description.ext
This shouldn't conflict with any other dialogs unless you are trying to use this in Wasteland (as the class names for the dialogs are the same as wasteland).
It is best to attach the action to a pre-existing ammo box so place a ammo box on the map via editor and in the initialization field put:

this addAction["<t color='#ff1111'>Virtual Ammobox</t>", "VAS\open.sqf"];

And your done! Just look at the ammo box, scroll and click Virtual Ammobox. The interface is easy to use so have fun!


Credits & thanks:
Kronzky - For his string function library
SaMatra - For help with UI Resources and Russian Translation
Dslyecxi - For his Paper doll giving insight on how to detect item types.
Tyrghen on Armaholic - For giving me the tip about CfgFunctions
naong - For his code tweaks to the Load / Save display.
Coding from armaholic - Translation of VAS from English->German
El nabot from Armaholic - Translation of VAS from English->French
czesiek77 from Armaholic - Translation of VAS from English->Polish
Ficc from BIS Forums - Translation of VAS from English->Portuguese
ramius86 on BIS Forums - Translation of VAS from English->Italian
RabsRincon on Armaholic - Translation of VAS from English->Spanish
Bakarda on BIS/Armaholic - Translation of VAS from English->Czech
MemphisBelle on BIS Forums - Translation Tweaks for German to fit.
Robalo on BIS Forums - Giving code changes to help support new compatibleItems class structure.