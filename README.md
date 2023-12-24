# Fantasia+
Fantasia+ is a Dalamud plugin designed to give you better control over your Final Fantasy XIV character appearance. Namely it allows you to apply character bone manipulations during gameplay.
Fantasia+ is a re-implementation of [Customize+](https://github.com/XIV-Tools/CustomizePlus) plugin.

### Changes compared to Customize+ (as of 1.0.0)
* Almost everything has been completely rewritten from scratch.
* New user interface similar to [Glamourer](https://github.com/Ottermandias/Glamourer).
* Template system. All bone edits are now stored in templates which can be used by multiple profiles and single profile can reference unlimited number of templates.
* Automated configuration backups.
* Compatible with Customize+
	* Your Customize+ settings are automatically carried over, original files are not touched in case you want to go back to using Customize+.
	* Mare Synchronos synchronization is cross compatible with original Customize+. You will see everyone and everyone will see you no matter which plugin combinations are being used.
	* Profile data and clipboard copies **ARE NOT** backwards compatible. Moving to Fantasia+ is a one way process.
	* Customize+ clipboard copies currently cannot be loaded, this will be addressed in one of the next releases.
* Fixed "Only owned" setting not working properly in several cases and renamed it to "Limit to my creatures".
* Fixed profiles "leaking" to other characters due to issues in the original Mare Synchronos integration implementation.
* Compatibility with cutscenes is improved, but that was not extensively tested.
* Profiles can be applied to summons, mounts and pets. Root scaling is not available for mounts for now.
* User interface issues related to different resolutions and font sizes should *mostly* not occur anymore.

### Installing
⚠ Make sure you don't have original Customize+ installed. Don't worry, removing it will not remove your settings and profiles. **If Fantasia+ detects Customize+ it will automatically turn itself off.**

After doing that add the following URL to the Dalamud Custom Plugin Repositories list:  
`https://raw.githubusercontent.com/RisaDev/DalamudPlugins/main/repo.json`
Then search for Fantasia+ in the plugin manager.

## FAQ

### How do I report an issue with Fantasia+?
Please join [Risa's Tools Discord](https://discord.gg/jXhQgv7qjy) to report issues with Fantasia+.

### Where do I learn how to use Fantasia+?
Most of the things should be self-explanatory, if you do need help you can join the [Risa's Tools Discord](https://discord.gg/jXhQgv7qjy) and ask in the appropriate channel.

### When will it be updated?
I am working on this when I have free time and have a desire to do so, therefore update schedule is "when I feel like it". Real life and paid employment take priority over this project.

### Source code availability
Source code will be made available at a later point in time.

### IPC
Right now IPC implements all features found in Customize+ which are required for Mare Synchronos integration to work. Features not used by Mare Synchronos are not implemented.
This IPC is considered obsolete and only available for compatibility with Mare Synchronos/Customize+. Breaking changes can be made at any time without a warning, so use at your own risk. 
In the future it will be expected for other plugins to use new IPC developed specifically for Fantasia+ from scratch.

### Acknowledgements
* User interface and general plugin architecture is heavily based on the code written as a part of [Glamourer](https://github.com/Ottermandias/Glamourer) and [OtterGui](https://github.com/Ottermandias/OtterGui/) projects. Original code is licensed under Apache License 2.0.
* Bone manipulation code is based on the code written as a part of [Customize+](https://github.com/XIV-Tools/CustomizePlus) project. Original code is licensed under MIT license.
* Some of the game object interaction code is copied from [Penumbra](https://github.com/xivdev/Penumbra) and [Glamourer](https://github.com/Ottermandias/Glamourer) projects.
