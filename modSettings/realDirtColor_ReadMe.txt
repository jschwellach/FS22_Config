-=[Real Dirt Color for FS22]=-

Author : ViperGTS96
---------------------------------------------------
---------------------------------------------------
---------------------------------------------------

10 Color settings to interpolate between.

-Brown Dirt
-Brown Mud
-Slurry/Digestate
-Manure
-Red Dirt
-Red Mud
-Lime
-Snow
-Grass
-Chaff

---------------------------------------------------
---------------------------------------------------
---------------------------------------------------

*Notes
----------
*Global "modSettings" folder is in the same directory as your savegame folder(s).


-For grass color to take affect, the vehicle must be around loose laying grass (fillplanes) or be in a "field" of grass. (due to field moisture etc..)


-Southern Maps use the "Red Dirt and Mud" instead of brown upon map name detection. These names can be added to the realDirtColor.xml file within your "modSettings" folder.


-Color Change Speed is adjustable via the realDirtColor.xml file ("<colorSettings speed = "0.005"/>") (Lower the value (slightly) to the slower the speed) within your "modSettings" folder.

---------------------------------------------------
---------------------------------------------------
---------------------------------------------------


-- Add the following to a vehicle xml to Override the maxNumOfWheels Limit..

  
  <realDirtColor ignoreRDCWheelLimit="true" />


---------------------------------------------------


-- Add the following to a vehicle xml to force simple mode to the vehicle/tool..

  
    <realDirtColor useSimpleMode="true" />

  
---------------------------------------------------

-- Add the following to a vehicle xml to disable Real Dirt Color for the vehicle/tool..
  
    <realDirtColor disable="true" />
    

---------------------------------------------------
---------------------------------------------------
---------------------------------------------------

*Modding with Real Dirt Color*
----------------------------

If vehicle parts are deleted/added during gameplay (not at a store or repair shop) then the part(s) needs to be removed/added to the vehicle's "Real Dirt Color" references. (Rare)

To remove a part call >>      realDirtColor:removePart(self, partToRemove);  *(This function will return "true" if the part was removed sucessfully, otherwise false)

To add a part call >>      realDirtColor:addPart(table, partToadd);

---------------------------------------------------
---------------------------------------------------
---------------------------------------------------