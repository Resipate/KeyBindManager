# KeyBindManager
This is a program that has been developed through Unity for the primary purpose of game development in the area of customising controls for the user.
This algorithm does not include any GUI aspects, however it would make the entire process of saving controls much easier.

# KeyBindManager Functions & Purpose
#### KeyBindManager.addBinding(string identifier, KeyCode keyCode)
This function is used to add a new binding to the list of bindings that exist, this will then update the file automatically meaning no other user action is required.

#### KeyBindManager.getBinding(string identifier)
This function is used to return the KeyCode associated with it. This is the main method of returning the KeyCode to implement into an input system.

#### KeyBindManager.removeBinding(string identifier)
This function is used to remove any one particular binding from the list.

#### KeyBindManager.changeBinding(string identifier, KeyCode newKeyCode)
This function is used to change a pre-existing bindings KeyCode without actually deleting the code itself. Could be used in a control changing GUI.

# Installation
To use this code, unpack the file and ensure both the KeyBind class, as well as the KeyBindManager class exist. Next up is to create a txt file in an area of your choosing and copy the datapath (in Unity, this can be done by right clicking the file and pressing "Copy Path"). Then in a place of your choosing, call the manager class with:

KeyBindManager newKBM = new KeyBindManager(string dataPath)

where "string dataPath" is the copied path of the txt file. Once that is complete, all the installation will be complete.

# Manually Inputting KeyBinds
It can be tedious to add each keybind through code, so an easy way to solve this is to just put it directly into the txt file and manipulate it from there. 
As such, this section is to provide the template of data. Below is the following template
#### identifier:keyCode
And here is a list of template keycodes for basic WASD movement for context
##### UP:W
##### DOWN:S
##### LEFT:A
##### RIGHT:D
These should occupy 1 line each with no spaces in between.
