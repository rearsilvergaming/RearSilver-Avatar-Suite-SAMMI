# RearSilver Avatar Suite for SAMMI

The official SAMMI integration for [RearSilver Avatar Suite](https://imperialinfusions.com/products/rearsilver-avatar-suite).

It connects SAMMI Bridge to Avatar Suite's local WebSocket server and provides commands to:

- Check that Avatar Suite is available and save its response as a SAMMI object
- Refresh the current Avatar Suite catalogue
- Activate a preset
- Show or hide a layer or group
- Switch configured effects on or off
- Run an ordered sequence of Avatar Suite actions

The extension includes an **Avatar Suite Examples** deck with buttons for checking the connection and refreshing the catalogue.

## Requirements

- RearSilver Avatar Suite running on the same Windows computer
- SAMMI with SAMMI Bridge
- Local connections to `ws://127.0.0.1:17891/`

Avatar Suite does not require Twitch credentials from SAMMI. The extension communicates only with the local Avatar Suite application.

## Installation

1. Download [`RearSilver Avatar Suite SAMMI.zip`](RearSilver%20Avatar%20Suite%20SAMMI.zip).
2. Extract `RearSilver Avatar Suite.sef` from the ZIP file.
3. Start RearSilver Avatar Suite.
4. Open SAMMI Core.
5. Choose **Bridge**, then **Install an Extension**.
6. Select the extracted `.sef` file.
7. Open the **RearSilver Avatar Suite** tab in SAMMI Bridge and confirm that it reports **Connected and verified**.
8. Accept the included example deck when SAMMI offers to install it.

Avatar Suite command selectors use the friendly preset, layer, group, and effect names from the currently active setup. They refresh automatically when Avatar Suite reports a catalogue change. A manual **Refresh Catalogue** command is also available.

## Check Server result

The **Check Server** command saves a structured object to the variable selected in **Save response as**. A successful response includes fields such as `ok`, `version`, and `protocolVersion`. A failed response returns `ok: false` with an `error` field.

## Privacy

The extension does not collect or transmit personal information. It connects only to Avatar Suite's local WebSocket server on the same computer. Avatar Suite's privacy information is available in the [RearSilver software privacy policy](https://imperialinfusions.com/pages/rearsilver-software-policy).

## Support

For help with Avatar Suite or this integration, contact [Imperial Infusions](https://imperialinfusions.com) or email `contact@imperialinfusions.com`.
