# BeamMP Linux Helper
Install instructions and script to launch BeamNG with the multiplayer mod.

![Screenshot of the BeamMP menu running on a Linux environment](/assets/screenshot_menu.png)

## Requirements
- BeamNG is installed in `~/.steam/steam/`
- Protontricks

## Installing BeamMP
1. Make sure you have installed BeamNG and run the game at least once.
2. Download the BeamMP client from the [BeamMP website](https://beammp.com/).
3. Extract the ZIP so you are left with `BeamMP_Installer.exe`.

4. Run Protontricks and select the BeamNG steam app. (Steam ID 284160)

![Screenshot of Protontricks select steam app window](/assets/screenshot_setup_steam_app.png)

5. Press "Select the default wineprefix".

![Screenshot of Protontricks select what you want to do window](/assets/screenshot_setup_select_wineprefix.png)

6. Press "Run explorer".

![Screenshot of Protontricks select what you want to do in the wineprefix window](/assets/screenshot_setup_select_run_explorer.png)

7. Navigate to the `BeamMP_Installer.exe` and double click the file to execute it.

![Screenshot of Protontricks explorer window](/assets/screenshot_setup_run_installer.png)

8. Follow the installer just like you normally would on Windows.

![Screenshot of the BeamMP installer window](/assets/screenshot_setup_installer.png)

## Running BeamMP
All you have to do, is run the `launch-beammp.sh` file located in this repository.
This should launch the game.

If you stored the game or Proton in a different location, you will have to modify the `launch-beammp.sh` script first to point it to the correct directories.

## Troubleshooting
If the game doesn't launch and you get an error, you can try to find it in this list and possible fixes.
Keep in mind that these are the error's that I've seen, please visit the [BeamMP wiki](https://wiki.beammp.com/en/) for more troubleshooting information.

### Command not found or Permission denied
If you get this error while trying to run `launch-beammp.sh`, you most likely forgot to add execution rights to the script.

#### Possible fixes
- Make sure that the `launch-beammp.sh` has execution rights.
    - These can be added using `chmod +x launch-beammp.sh`
    - Or alternatively, using your desktop environment by right clicking the file and going to Properties -> Permissions -> Is executable.

### Failed to find the game please launch it. Report this if the issue persists code X
According to the [BeamMP wiki](https://wiki.beammp.com/en/error-codes), this error means that the launcher was unable to find or read the game's info inside the registery.

#### Possible fixes
- Make sure that the Proton version matches that of your BeamNG install.
- Make sure that you have actually launched the game at least once before.
