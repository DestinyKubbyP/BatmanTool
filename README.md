# BatmanTool

Hello I am DestinyTakes and this is my tool for batman arkam series. This allows major game overhauls and the acsess to cheats and fun modifiers.
This is supported throuhout all the game series. My main goal is to make the game more smooth and add new unique ablities. Ive already dumped many many hours in disecting there game engine.
They use verison of unreal engine mixed with variants of other engines, but all that is important to me is the base game engine where the major game events are located. Disecting Unreal Engine is very annoying and totaly a horrible idea if your new to this scene.
If you do not have proper reversing experince this may be very confusing and a horrible dev log for you to read.

# Engine Overview
### Engine : Unreal Engine
### FNAME : A fname is a entry for a object for its name. This is so the engine can do optimized creation and indexing of strings to avoid using more resourses. 
### UOBJECT : A UObject is a object entry that all classes inheirt within unreal engine contains a fname index.
### ENGINEPTR: This is the main engine array where all game contents are stored.
### UOBJECTLIST: This is where all game objects are stored and what will allow us to map all game classes properly do to the static non active objects being stored there. For easy future function use. Can be found in the world of the engine pointer.
### PROCESSEVENT: This is a major function used in all unreal engine games that process game events. Hooking this event can help use alter incoming game behvoir from the BMScript clients.

## These are just some defientions I may use so read up on these. Unreal engine is actually pretty simple and straight foward to take on once you understand and retrace to a form of UOBJECTLIST or ENGINEPTR and map these structures to the FNAME ENTRY ARRAY. To properly map objects so we can deeply understand there data types and properly use them. 
