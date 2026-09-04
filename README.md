# Quicker Connect Button (Fork)

This is a fork of [Quicker Connect Button](https://github.com/JamCoreModding/quicker-connect-button) updated for **Minecraft 26.2** and **Fabric Loader 0.19.5**.

> [!NOTE]
> This fork is tested **only on Fabric**. Compatibility with NeoForge is not guaranteed and disabled in this build.

## Download
You can find the latest releases in the [Releases](https://github.com/CelduinX/quicker-connect-button/releases) tab.

## Configuration

The config can either be changed through a GUI (using Mod Menu on Fabric or the config button on Forge), or directly at `config/quickerconnectbutton.json5`. The GUI contains tooltips explaining each option.

```json5
{
  /* Leave empty to disable the quick connect button
     - default: \"\"
  */
  ip: "localhost",
  /* - default: 25565
     - must be between 0.0 and 65535.0
  */
  port: 25565,
  /* Where to place the connect button
     - default: RIGHT
     - must be one of: RIGHT, REPLACE_MULTIPLAYER_BUTTON, REPLACE_SINGLEPLAYER_BUTTON, REPLACE_REALMS_BUTTON
  */
  buttonLocation: "REPLACE_MULTIPLAYER_BUTTON",
  /* The text to display on the button. Leave empty to use "Connect".
     - default: \"\"
  */
  text: "Connect to an Awesome Server",
  /* What to do if the server has a resource pack.
     - default: PROMPT
     - must be one of: ENABLED, DISABLED, PROMPT
  */
  resourcePackBehaviour: "ENABLED"
}
```

[![Rent a server with Bisect Hosting: Use Code jamalam to get 25% off](https://www.bisecthosting.com/partners/custom-banners/e0cc6668-0d29-40ff-9820-4d4f5433198a.webp)](https://bisecthosting.com/jamalam)
