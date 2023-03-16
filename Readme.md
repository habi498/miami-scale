Instructions 
============
Put miamiscale04relxx in plugins folder and vicecity.map in server directory.

Use MiamiScale_Init("vicecity.map"); //when it is placed in server directory.

Use MiamiScale_Unload to unload it.

It uses approximately 50 MB of RAM when Init.


Functions
=========
[true on success] MiamiScale_Init([string]mappath)  
[true|false]MiamiScale_Unload();  
[float|null]FindZFor2DCoord([float|integer]x, [float|integer]y);  
[float|null]FindAverageZ([float|integer]x, [float|integer]y);  
[true on success]SetZFor2DCoord([integer]x, [integer]y, [float]z);  
[true on success]MiamiScale_SaveCurrentMap([string]filename);  

Note
-------
Saving Map takes approximately 2 seconds.
