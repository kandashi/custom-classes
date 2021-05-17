# Custom Classes 

Custom Classes allows you to relatively easily add features to auto-apply on leveling up in DnD5e. Simply edit the `module.js` file with the required links to compendium items at the appropriate level and refresh browser to load in the changes.

The command `CustomClasses.exportList()` will save a txt file with all the names and IDs of the items within the Custom Classes Class Features compendium pack, for easy referencing.

Simply format your feature lists as follows:

### Class Features
```
"features": {           //each level should be an Array [], containing a String ("") of the item, separated by commas
                "1": ["Compendium.dnd5e.classfeatures.VoR0SUrNX5EJVPIO", "Compendium.dnd5e.classfeatures.SZbsNbaxFFGwBpNK"],
                "2": ["Compendium.dnd5e.classfeatures.SCVjqRdlZ9cvHVSR", "Compendium.dnd5e.classfeatures.vt31lWAULygEl7yk"],
```

### Sub Class Features
```
"path-of-the-berserker": {
                    "label": "Path of the Berserker", // name of the subclass here, this is case in-sensitive
                    "source": "PHB pg. 49",     // this is purely descriptive
                    "features": {      //each level should be an Array [], containing a String ("") of the item, separated by commas
                        "3": [
                            "Compendium.dnd5e.classfeatures.CkbbAckeCtyHXEnL",
                            "Compendium.dnd5e.classfeatures.0Jgf8fYY2ExwgQpN"
                        ], 
                        "6": ["Compendium.dnd5e.classfeatures.0Jgf8fYY2ExwgQpN"],
                        "10": ["Compendium.dnd5e.classfeatures.M6VSMzVtKPhh8B0i"],
                        "14": ["Compendium.dnd5e.classfeatures.xzD9zlRP6dUxCtCl"]
                    }
                },
```

