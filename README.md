# NoteTweaks
This is a Beat Saber mod that lets you tweak various aspects of the default note.

> [!NOTE]
> **This is currently actively maintained for the latest version of the game.**

# Personal note
> I will not be adding any features to this mod. I've had multiple people reach out asking if this mod would continue to receive updates (at least to keep it working), and it doesn't feel fair to just drop support for an accessibility mod the way I did back in August 2025. I do not regret the things I said/did about that one DITR map that ended up being the straw that broke my back.
>
> **To the Beat Saber modding community**: don't bother to submit any PR's or try to fix things and hand them back to this repository. I do not trust any of you to not use generative AI tools. PR's are off.
>
> **To the Beat Saber community *at large***: fuck you, fuck off. You'll know if this is directed at you or not.

## Downloads
See the [releases page](https://github.com/TheBlackParrot/NoteTweaks-LifeSupport/releases) for mod downloads.

## Heads up!
- It is recommended to disable other mods that also change aspects of the default note if you want to use this mod, as conflicts *can* occur.
  - The Custom Notes mod does not appear to cause any conflicts, should be fine.
  - Some users have reported that NalulunaNoteDecor causes some conflicts, although I haven't seen any issues crop up with it. ~~(ymmv)~~
- Face symbols are forced to their default colors if the *Ghost Notes* modifier is enabled.

## Configuration
Configuration is done in-game via a Menu button in the left panel of the Main Menu, or by editing `UserData/NoteTweaks.json`.  
Presets can also be saved/loaded in-game via the menu on the right in the settings menu.

## Custom Cubemap textures
Cubemap textures can be changed on notes and bombs; NoteTweaks will pull individual face textures from folders in `UserData/NoteTweaks/Textures/Notes`, and can dynamically generate a cubemap from a single texture as well.

Each folder should have a **512x512** image **(in `.jpg`, `.png`, or `.tga`)** for each side of a cube:
- `nx` *(left)*
- `ny` *(bottom)*
- `nz` *(back)*
- `px` *(right)*
- `py` *(top)*
- `pz` *(front)*

If any images are missing, or if an image is not any of the expected filetypes, the folder will not be selectable in-game.

Individual images outside of folders can also be selected.

I've provided [36 cubemap textures](https://github.com/TheBlackParrot/NoteTweaks/releases/download/0.5.0/Note.Cubemap.Textures.zip) that you can use with the mod, ready-to-go. If you want to convert a panoramic image, [Kyle Nguyen's Optifine Sky Generator](https://skybox-generator.vercel.app) is an easy online tool to split the image into 6 cube faces. *(use a 2048x1024 image to get 512x512 face textures, no post-resizing needed)*

## Dependencies
- BSIPA
- BeatSaberMarkupLanguage
- SiraUtil
- SongCore

## Reference Mods
- BeatLeader
- BSExtraColorPresets
- SoundReplacer *(Meivyn's fork)*
- BeatSaberPlus
- JDFixer
- CustomNotes
- CustomSabersLite
- Camera2
- BetterSongSearch
- ImageFactory *(DJDavid98's fork)*
- SaberFactory
- NoteMovementFix
- BS Utils
