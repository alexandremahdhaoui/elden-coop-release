# Elden Coop

Play one Elden Ring world together with friends. Elden Coop is in early development and these builds are for early testing, so expect crashes and missing features. It is an open source project, and the source goes public later.

## Install

1. Open Steam and sign in. You need Elden Ring version 2.7.2.0.
2. Download `EldenCoop.exe` from the [newest release](https://github.com/alexandremahdhaoui/elden-coop-release/releases/latest).
3. Double click it. If Windows warns you about an unknown publisher, click More info, then Run anyway.
4. Approve the Windows admin prompt the first time it appears.
5. Press Play.

The launcher finds the game through Steam, installs the mod and updates itself. It only installs builds with a valid Elden Coop signature.

Step 4 is the only time the launcher asks for admin rights. It adds the Elden Coop certificate, so this PC trusts code that Elden Coop signs. Approve it only if you trust the person who sent you here.

## Join a friend

1. Wait on the title menu for a Steam invite from your host.
2. Press Shift and Tab to open the Steam overlay, then accept the invite.
3. In the game, pick MULTIPLAYER, then JOIN A WORLD, then JOIN FROM A STEAM INVITE.
4. Pick CREATE A CHARACTER and finish the character creator.
5. Stay in the game when you reach the world. The mod joins the host by itself.

Use only the MULTIPLAYER menu, and do not press Escape on the title screen.

## Your saves

The mod keeps its own saves in a separate folder and refuses to open your normal save.

Before each game, the launcher copies every changed file from `%APPDATA%\EldenRing` to the `EldenCoop-backups` folder in your user folder. It keeps the older copies. It never deletes a save and has no restore feature. If something goes wrong, ask your host before you touch these files.

## If Windows blocks the launcher

Use this if `EldenCoop.exe` will not open or step 4 failed. Open Windows Terminal as administrator, paste this block, then double click `EldenCoop.exe` again.

```powershell
$base = "https://github.com/alexandremahdhaoui/elden-coop-release/releases/latest/download"
Invoke-WebRequest "$base/EldenCoop-root.cer" -OutFile "$env:TEMP\EldenCoop-root.cer"
Invoke-WebRequest "$base/EldenCoop-publisher.cer" -OutFile "$env:TEMP\EldenCoop-publisher.cer"
Import-Certificate -FilePath "$env:TEMP\EldenCoop-root.cer" -CertStoreLocation Cert:\LocalMachine\Root
Import-Certificate -FilePath "$env:TEMP\EldenCoop-publisher.cer" -CertStoreLocation Cert:\LocalMachine\TrustedPublisher
```

## Report a problem

Press Save a diagnostic report in the launcher. It saves one zip with the logs of your last five runs on your Desktop, then opens the folder. The zip stays on your PC until you send it to your host by hand.

## Uninstall

1. Press Remove the certificate in the launcher and approve the Windows prompt.
2. Delete `EldenCoop.exe`.
3. Delete the `EldenCoop` folder from the `Game` folder of Elden Ring.

To play the normal game, start it from Steam as usual.

## License

Elden Coop uses the Apache License 2.0 in `LICENSE`, limited by `LICENSE-ADDENDUM.md`. The license covers the launcher, the mod code and the methods of this project. It never covers Elden Ring or anything that belongs to FromSoftware.
