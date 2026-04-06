# Obrero
Obrero Develop Language Repository for Chimo Linux Cinder and above
🔗 Obrero Language

The Heavy-Duty Logic for Chimo Linux

Obrero is a high-level, human-readable programming language designed for Chimo Linux. It follows a "Noun + Verb" logic, making it the most intuitive engine for building Apps, 2D Games, and Robotics without the complexity of traditional syntax.
🚀 Core Philosophy

    Simple Syntax: No brackets, no complex pointers. Just English commands.

    Unified Logic: The same commands work for a simple "Hello World" and a complex Neural Network or Robot.

    CHX Integration: Native support for the .chx package manager and Setup Wizard.

🛠 Command Reference
1. Project Initialization
Command	Description	Example
create "scenario"	Initializes the graphics engine and main window.	create "scenario"
window W, H	Sets the custom resolution of the application.	window 1280, 720
paint R, G, B	Fills the background with an RGB color.	paint 255, 0, 0
2. Object Management
Command	Description	Example
load "file" as "id"	Links an asset (GIF, PNG, MP3) to a nickname.	load "hero.gif" as "player"
put "id"	Places the object into the active scenario.	put "player"
add "A" on "B"	Links two objects or features together.	add "sword" on "hand"
3. Logic & Control
Command	Description	Example
move with "ctrl" the "id"	Maps input (keys/mouse) to an object.	move with "keys" the "player"
set "var" to "val"	Stores data in the application memory.	set "score" to "100"
if "X" is "Y" do "Z"	Conditional logic for decision making.	if "life" is "0" do "exit"
wait SEC	Pauses execution for a specific time.	wait 2
4. Storage & Persistence
Command	Description	Example
save "ctx" to "storage"	Permanently saves all variables to a local file.	save "ctx" to "storage"
load "storage" to "ctx"	Retrieves saved data upon app launch.	load "storage" to "ctx"
write "str" on "file"	Appends text to a specific document.	write "Log" on "save.txt"
5. System & UI
Command	Description	Example
say "message"	Prints text to the console/debug log.	say "App Started"
popup	Triggers the ChimoPods/JBL system interface.	popup
exit	Safely closes the application.	exit
🎮 Game Example: "Surfer Adventure"
Python

~~ Obrero Game Script ~~
create "scenario"
window 1280, 720
load "ocean.gif" as "bg"
load "surfer.gif" as "hero"

put "bg"
put "hero" at 400, 300

move with "direction_keys" the "hero"
if "hero" hits "virus" do "exit"

say "Surfing the Network..."

📦 How to Build & Install

Obrero scripts (main.obr) must be compiled using the CHX Manager.

    Pack the project:
    Bash

chx pack my_project_folder -o app_name.chx

Install via Wizard:
Double-click the .chx file or run:
Bash

    chx-gui app_name.chx

🏗 Requirements

    Chimo Linux (Any version: Córdoba, Ruby, Artemis, etc.)

    Python 3.10+

    PyQt6 & Pygame (Handled automatically by CHX)

Developed by Franco Peruzzi Outstanding Personality for Autism Day Chimo Inc. & Chimo Linux Founder
