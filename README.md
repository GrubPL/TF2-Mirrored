# Team Fortress 2 Mirrored

Source code for Team Fortress 2 Mirrored

A Team Fortress 2 Sourcemod that mirrors the game

It has an issue with some hud elements not getting mirrored, most seen with the health bar that appears above players when hovering over them, the hp/name indicators that appear whenever you spawn in/are in spectator, and damage numbers

and with my lack of coding experience, I doubt i'll be able to fix it by myself

## Credits

NvC-DmN-CH - Half-Life 2 Mirrored Source code https://github.com/NvC-DmN-CH/Half-Life-2-Mirrored

## Build instructions

Clone the repository using the following command:

`git clone https://github.com/GrubPL/TF2-Mirrored`

### Windows

Requirements:
 - Source SDK 2013 Multiplayer installed via Steam
 - Visual Studio 2022 with the following workload and components:
   - Desktop development with C++:
     - MSVC v143 - VS 2022 C++ x64/x86 build tools (Latest)
     - Windows 11 SDK (10.0.22621.0) or Windows 10 SDK (10.0.19041.1)
 - Python 3.13 or later

Inside the cloned directory, navigate to `src`, run:
```bat
creategameprojects.bat
```
This will generate the Visual Studio project `tf2_mirrored.sln` which will be used to build TF2 Mirrored.

Then, on the menu bar, go to `Build > Build Solution`, and wait for everything to build.

You can then select the `Client (Mod Name)` project you wish to run, right click and select `Set as Startup Project` and hit the big green `> Local Windows Debugger` button on the tool bar in order to launch your mod.

The default launch options should be already filled in for the `Release` configuration.

### Linux (Not Tested For TF2:M)

Requirements:
 - Source SDK 2013 Multiplayer installed via Steam
 - podman

Inside the cloned directory, navigate to `src`, run:
```bash
./creategameprojects
```

This will build all the projects related to the SDK and your mods automatically against the Steam Runtime.

You can then, in the root of the cloned directory, you can navigate to `game` and run your mod by launching the build launcher for your mod project, eg:
```bash
./mod_tf
```

## License

The SDK is licensed to users on a non-commercial basis under the [SOURCE 1 SDK LICENSE](LICENSE), which is contained in the [LICENSE](LICENSE) file in the root of the repository.

For more information, see [Distributing your Mod](#markdown-header-distributing-your-mod).
