Basically, you to use this you need: Windows, RCON and some basic Zomboid server knowledge.

Download the required tools:

RCON client: Download the RCON client from https://github.com/gorcon/rcon-cli/releases/tag/v0.10.1 and place the executable (rcon.exe) in a convenient location.
Scripts: Download the scripts from '' and extract them to a folder of your choice. Make sure to note the file paths where you place these scripts.
Set up RCON on your server:

Run the RCON Client (rcon.exe) and set up your IP (127.0 0.1 is the local IP) and password.
Modify the scripts:

Open the 30m.bat, 20m.bat, 10m.bat, 5m.bat, 1m.bat, quit.bat, and StartServer64.bat files using a text editor.
Inside each of the RCON scripts (30m.bat, 20m.bat, 10m.bat, 5m.bat, 1m.bat, quit.bat) replace the string "password" with your actual RCON password.
In StartServer64.bat, modify the file paths to match the location of the RCON client (rcon.exe) and the other RCON scripts (30m.bat, 20m.bat, 10m.bat, 5m.bat, 1m.bat, quit.bat).
Replace the default script:

Locate the default script file (StartServer64.bat) in your dedicated server installation directory.
Replace the default script with the modified StartServer64.bat file from the extracted folder.
Delete the workshop manifest file:

Locate the appworkshop_108600.acf file inside the dedicated server installation directory.
Delete the appworkshop_108600.acf file.
Start the server:

Launch the Project Zomboid dedicated server using the modified StartServer64.bat script.
With these steps, your Project Zomboid server will automatically send restart warnings to players at 10 minutes and 1 minute intervals before cleanly restarting the server. The process will repeat in a continuous loop.

Found this on Reddit and edited it a bit: https://github.com/MonkeyyNinja/PZ-AutoRestart
