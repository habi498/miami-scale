Instructions 
============
Put miamiscale04relxx in plugins folder and vicecity.map in server directory.

Use MiamiScale_Init("vicecity.map"); //when it is placed in server directory.

Use MiamiScale_Unload to unload it.

It uses approximately 50 MB of RAM when Init.


Functions
=========
| Return value    | Function Name             | Parameter                            | Description                                                                                                                |
|-----------------|---------------------------|--------------------------------------|----------------------------------------------------------------------------------------------------------------------------|
| true on success | MiamiScale_Init           | [string] mapfile                     | The full path to mapfile as parameter                                                                                      |
| true or null    |     MiamiScale_Unload     | -                                    |                                                                                                                            |
| float or null.  | FindZFor2DCoord           | [float\|integer]x, [float\|integer]y | The x,y co-ordinates to find the corresponding z. Return value null means z does not exist - it might be sea or something. |
| float or null   | FindAverageZ              | [float\|integer]x, [float\|integer]y | same as above                                                                                                              |
| true on success | SetZFor2DCoord            | [integer]x, [integer]y, [float]z     | Sets the z co-ordinate for a certain pair of integer x,y co-ordinates. Setting means subsequent get will fetch this value. |
| true on success | MiamiScale_SaveCurrentMap | [string]filename                     | Saves the current map which might have changes resulting from function mentioned in above row.                             |

Note
-------
Saving Map takes approximately 2 seconds.
