# Elden Coop lets friends play one Elden Ring world together

Elden Coop is in early development, and the builds in this repository are for early testing. Expect crashes and missing features. Elden Coop is an open source project. Its source repositories are not public yet, and they go public later.

## One file installs and starts the mod

1. Open Steam and sign in. You need Elden Ring version 2.7.2.0.
2. Download `EldenCoop.exe` from the [newest release](https://github.com/alexandremahdhaoui/elden-coop-release/releases/latest).
3. Double click `EldenCoop.exe`. Windows may warn you about an unknown publisher. Click More info, then Run anyway.
4. Press TRUST THE ELDEN COOP CERTIFICATE and approve the Windows prompt.
5. Press PLAY.

The launcher finds the game through Steam and installs the mod in the game folder. It updates itself when a new build comes out, and it only installs a build that carries a valid Elden Coop signature. The launcher asks for admin approval only in step 4, and it never runs as admin otherwise.

## Trusting the certificate gives this PC a new root

Step 4 adds the Elden Coop root certificate to Windows. This PC then trusts code that Elden Coop signs, so only do this if you trust the person who sent you here. The launcher shows REMOVE THE CERTIFICATE to undo it.

## Windows Smart App Control needs one extra step

Smart App Control can block `EldenCoop.exe` before the launcher opens, so the button in step 4 cannot help. Open Windows Terminal as administrator, paste this block, then double click `EldenCoop.exe` again.

```powershell
$base = "https://github.com/alexandremahdhaoui/elden-coop-release/releases/latest/download"
Invoke-WebRequest "$base/EldenCoop-root.cer" -OutFile "$env:TEMP\EldenCoop-root.cer"
Invoke-WebRequest "$base/EldenCoop-publisher.cer" -OutFile "$env:TEMP\EldenCoop-publisher.cer"
Import-Certificate -FilePath "$env:TEMP\EldenCoop-root.cer" -CertStoreLocation Cert:\LocalMachine\Root
Import-Certificate -FilePath "$env:TEMP\EldenCoop-publisher.cer" -CertStoreLocation Cert:\LocalMachine\TrustedPublisher
```

## Your normal save stays safe

The mod keeps its own saves in a separate folder and refuses to open the normal save. Use only the MULTIPLAYER menu in the game. Do not press Escape on the title screen.

## A host invites you through Steam

1. The host sends you a Steam invite while your game sits on the title menu.
2. Press Shift and Tab to open the Steam overlay, then accept the invite.
3. In the game pick MULTIPLAYER, then JOIN A WORLD, then JOIN FROM A STEAM INVITE.
4. Pick CREATE A CHARACTER and finish the character creator.
5. Stay in the game when you reach the world. The mod joins the host by itself.

## A report helps fix a problem

Press SAVE A DIAGNOSTIC REPORT in the launcher. The launcher saves one zip on your Desktop and opens the folder for you. The zip holds the logs of the last five runs. It stays on your PC until you send it to your host by hand.

## Removing the mod takes three steps

1. Press REMOVE THE CERTIFICATE in the launcher and approve the Windows prompt.
2. Delete `EldenCoop.exe`.
3. Delete the `EldenCoop` folder from the `Game` folder of Elden Ring.

Start the game from Steam as usual to play the normal game.

## The license covers only the work of this project

Elden Coop uses the Apache License 2.0 in `LICENSE`, limited by `LICENSE-ADDENDUM.md`. The license covers the launcher, the mod code and the methods of this project. It never covers Elden Ring or anything that belongs to FromSoftware.
