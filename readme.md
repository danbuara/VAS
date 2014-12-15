<p align="center">
  <h1 align="center">Virtual Ammobox System</h3><br />
  <a href="https://raw.githubusercontent.com/TAWTonic/VAS/master/changelog.txt">
    <img src="http://img.shields.io/badge/Version-2.6-green.svg?style=flat" alt="VAS changelog">
  </a>
    <a href="http://www.armaholic.com/page.php?id=19134">
    <img src="http://img.shields.io/badge/Download-1_MB-blue.svg?style=flat" alt="VAS download">
  </a>
    <a href="#license">
    <img src="http://img.shields.io/badge/License-Custom-red.svg?style=flat" alt="VAS license">
  </a>
</p>

Thank you for using Virtual Ammobox System (VAS). This script allows you to equip, configure and customize the default loadout gear using an easy to use GUI.

VAS was originally written by [Tonic](https://github.com/TAWTonic) to compliment the release of only one particular Arma 3 mission. However, after the script's initial success and a wide adoption within community, he made the source code to VAS available publicly - for everyone to use, modify and contribute to its ongoing development.

###Goals
* Provide a viable alternative to the native solution from [BIS](https://www.bistudio.com/).
* Cut back on the time spent browsing in-game inventory.
* Deal with the associated lag issues.

###Installation
The script is very easy to integrate. To add VAS to your mission, simply copy it to your mission folder and edit out your **description.ext** with the following:
```
#include "VAS\menu.hpp"  
  
class CfgFunctions  
{  
	#include "VAS\cfgfunctions.hpp"  
};
```
This inclusion shouldn't conflict with any existing dialogs, perhaps with the exception of Wasteland where the default class names are identical to VAS.  

I would recommend attaching the VAS menu to a pre-existing ammunition box, so when you place an ammobox in map via editor, add the following into its initialization field:
```
this addAction["<t color='#ff1111'>Virtual Ammobox</t>", "VAS\open.sqf"];
```
That's it! Now when you look at your new ammunition box in-game, the mouse-wheel menu will present you with the "Virtual Ammobox" item. The underlying interface is localized into 8 languages, and is intuitive enough to skip the introductions.

###License <a name="license"></a>
Use of Virtual Ammobox System (VAS) in missions published on [Steam Workshop](http://steamcommunity.com/app/107410/workshop/?l=english) is allowed. Publishing the script by itself is prohibited.

VAS is intended for mission designers to be integrated into their own work, and is not to be released separately (as is) via the Workshop or elsewhere.

###Special Thanks
* [Dslyecxi](http://dslyecxi.com/) for his Paper Doll script, giving me insight on how to detect item types.
* [Kronzky](http://www.kronzky.info/) for his string function library.
* [Robalo](http://arma-sr.bzbit.com/) for providing code changes to help support the new compatibleItems class structure.  
* [Tyrghen](http://veterans.armasites.com/) for the tip on CfgFunctions.
* [naong](http://www.armaholic.com/forums.php?m=posts&id=142583) for his code tweaks to the Load/Save display.  
* [Sa-Matra](https://wasteland.arma.su/) - For help with UI resources and Russian translation.
  * [PR9INICHEK](https://github.com/PR9INICHEK) & [Tourorist](https://github.com/Tourorist) for updates and additions to the Russian localization.
* [Coding](http://www.armaholic.com/forums.php?m=posts&id=149222) for translating VAS into German.
  * [MemphisBelle](https://twitter.com/MemphisBelle291) for tweaks to the German translation.
* [El nabot](http://www.armaholic.com/forums.php?m=posts&q=20990&d=105) for French translation.
* [czesiek77](http://instagram.com/czesiek77) for Polish translation.
* [Ficc](http://www.rifleonlyclan.com/) for Portuguese translation.
* [ramius86](https://github.com/ramius86) for Italian translation.
* [RabsRincon](http://www.armaholic.com/forums.php?m=posts&q=24317) for Spanish translation.
* [Bakarda](https://www.youtube.com/user/Bakarda/) for Czech translation.

The list goes on, sorry if I missed anyone out (let me know)!
