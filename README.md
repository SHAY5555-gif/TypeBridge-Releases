# TypeBridge downloads

TypeBridge connects Android dictation to a Windows PC. You can review the draft on the phone and insert the approved text into the selected desktop field.

[Download the latest release](https://github.com/SHAY5555-gif/TypeBridge-Releases/releases/latest)

| Download | Use |
| --- | --- |
| Android APK | Install directly on Android 8.0 or later. To update an existing direct installation, keep its data and check the signing certificate. A Play installation may use a different certificate. |
| Windows x64 installer | Install the desktop app for the current user. The installer is unsigned. |
| Windows x64 portable ZIP | Extract the folder and run TypeBridge.exe. Keep the bundled runtime, libraries and license notices together. |

## Connect to your computer

1. Open TypeBridge on Windows and open the phone connection screen. Choose **חיבור מוצפן ישירות למחשב** and the connection duration.
2. Scan that QR code from TypeBridge on Android. It contains the public key of the computer displaying it.
3. Leave the computer running. Dictate on the phone, review your draft, select the destination field on the PC, and send.

In this mode the phone encrypts audio and text for the PC. A relay forwards the encrypted packets. The PC decrypts them and uses its configured transcription providers. A disconnected computer cannot receive text. A signed-in user can explicitly select standalone cloud processing in phone settings. In standalone mode the hosted service and the selected providers process the content. Other users and guests keep their transcription history on their devices.

## Verify a download

Open the release's SHA256SUMS.txt and compare the hash of your download. On Windows, `Get-FileHash -Algorithm SHA256 <file>` prints the hash. The release manifest records the source build commit, Android application ID and signer. This repository publishes distribution files and their verification information.
