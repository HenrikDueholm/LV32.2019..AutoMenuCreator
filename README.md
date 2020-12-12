# LV32.2019..AutoMenuCreator
Scan a folder and Create menu files for the folder. Can also handle entire folder hierarchies using targets such as a .git folder to detect which folders to handle.
A config file is generated in each target folder that configures the menu generation for that folder.

Supports exclusions, inclusions and filters of various types.
Can assign icons to folders by name and path matching.
Can setup default configurations for palettes and files and individual configurations for palettes and files when there are deviations from the default.

Examine the data\Menu Config Template.ini to see how to do the configurations. 
Always use AutomMenu on a folder the first time to create the config file, then make changes and run it again.

Using the section "Main" and key "Relative Link Target" link and unlink bat files will be created in the menu folder that can link to a target relative folder inside of the '<Labview>\menus\Categories'-folder.
The feature is disabled if an empty key is provided. The "Auto Link"-key can be used to automatically refresh linked palette files on rebuild using the created bat-files.

# Test
To test the functionality of this repository:
1) Open: _Test\PPL Test.lvproj
2) Open: Test_Single folder menu refresh.vi
3) Set target folder and run the VI
4) Open: [target folder]\AutoMenu Config.ini
5) Configure to desired settings and setup folder icons
6) Rerun Test_Single folder menu refresh.vi to apply changes
7) Copy or link the 'Menu Folder' (default '_Menu') into desired location in [Labview]\Menus hierarchy or add it manually.

# Contribute:
Contact me at henrikdue at yahoo.dk.