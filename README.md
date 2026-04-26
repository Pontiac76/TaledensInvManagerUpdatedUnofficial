# TaledensInvManagerUpdatedUnofficial 

When you upload a script for the first time a new file "modinfo.sbmi" is created in folder that contains your script. The modinfo.sbmi file holds your steam user id and the workshop id.

If you try to update your script with create from editor, delete your old script and rename your newly created from editor script you will not be able to update the script unless you make a new modinfo.sbmi to match that workshop id. If you browse the workshop you can look at the URL anatomy for your script and take the workshop the portion following the "id=" is the workshop id.

http://steamcommunity.com/sharedfiles/filedetails/?id=########
Take that ID and make a new modinfo.sbmi in

%appdata%\SpaceEngineers\IngameScripts\local\SCRIPTNAME
example modinfo.sbmi

<?xml version="1.0"?>
<MyObjectBuilder_ModInfo xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
  <SteamIDOwner>###############</SteamIDOwner>
  <WorkshopId>0</WorkshopId>
  <WorkshopIds>
    <WorkshopId>
      <Id>###########</Id>
      <ServiceName>Steam</ServiceName>
    </WorkshopId>
  </WorkshopIds>
</MyObjectBuilder_ModInfo>

Simply replace the # symbols in the SteamIDOwner and WorkshopId elements to match your info!



To Make the process easier just create new script, copy the one from the workshop and then publish it. After that go to 
%appdata%\SpaceEngineers\IngameScripts\local\SCRIPTNAME
and just edit modinfo.sbmi, 
!! DONT FORGET TO COPY YOUR ORIGINAL SCRIPT WHEN PUBLISHING, AFTER THIS UPDATE YOU WILL LOOSE OLD SCRIPT AND REPLACE IT WITH THIS ONE!!!
