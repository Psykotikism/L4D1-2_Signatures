# L4D1&2 Signatures

## PayPal
[Donate to Motivate](https://paypal.me/Psyk0tikism?locale.x=en_US)

## About
This is a repository for hosting/storing several L4D1&2 signatures. More signatures will be added and supported as I come across or use more functions. I will try my best to keep all the signatures in this repository up-to-date.
1. If you want me to add/support any function that isn't in this repository already, file an issue.
2. If you have some signatures you want to share, make a pull request.
- Be sure to state which game the signatures are from.
3. If you encounter any bad/broken signatures, file an issue.
- Mention the game and platform.
4. Any signature that's broken by a game update will usually be fixed within 24 hours, so please allow at least that much time to pass before filing an issue.
5. If you encounter any signature that doesn't work on late plugin loads, file an issue.
- This usually only happens when another plugin detours or patches something in the same function.

## Files
1. `l4d1/raw/l4d1_signatures_linux.txt` - List of L4D1 Linux signatures
2. `l4d1/raw/l4d1_signatures_mac.txt` - List of L4D1 Mac signatures
3. `l4d1/raw/l4d1_signatures_windows.txt` - List of L4D1 Windows signatures
4. `l4d1/gamedata/l4d1_signatures.txt`
- Gamedata file that contains all of the signatures listed in the above files.
- Includes instructions for finding each signature.
5. `l4d2/raw/l4d2_signatures_linux.txt` - List of L4D2 Linux signatures
6. `l4d2/raw/l4d2_signatures_mac.txt` - List of L4D2 Mac signatures
7. `l4d2/raw/l4d2_signatures_windows.txt` - List of L4D2 Windows signatures
8. `l4d2/gamedata/l4d2_signatures.txt`
- Gamedata file that contains all of the signatures listed in the above files.
- Includes instructions for finding each signature.
9. `gamedata/l4d_signatures.txt`
- Gamedata file that contains all of the signatures for both games listed in the above files.
- Includes instructions for finding each signature.

## Notes

### General
- Most of these signatures are designed for detours since that is the only reason I sought most them in the first place. You can of course still use them for `SDKCall`'s and/or `Addresses`.
- Keep in mind that most plugins that are still being maintained already use up-to-date signatures, so unless you are getting errors for any of these functions, you do not need to use any of these signatures.
- Most of these signatures are heavily wildcarded but have been tested across multiple versions of both games to be very durable. While shorter signatures are ideal, longer but durable ones are more convenient.

### Signature Count
- **L4D1**: Linux/Windows - 292, Mac - 287
- **L4D2**: Linux/Windows - 405, Mac - 391

### Left 4 Dead
- Most of the signatures have been verified to have withstood the last landmark update:
1. `Old (7-24-2019)`
- `25/292` Windows signatures changed since the latest version came out.
- `3/292` Linux signatures changed since the latest version came out.
2. `Pre-Current (8-9-2021)`
- `3/292` Linux signatures changed since the latest version came out.
3. `Current (1-31-2022)`

### Left 4 Dead 2
- Most of the signatures have been verified to have withstood the last five landmark updates:
1. `Pre-TLS (6-5-2020)`
- `64/405` Windows signatures changed since the latest version came out.
- `8/405` Linux signatures changed since the latest version came out.
2. `TLS (9-24-2020)`
- `60/405` Windows signatures changed since the latest version came out.
- `5/405` Linux signatures changed since the latest version came out.
3. `Post-TLS (2-18-2021)`
- `57/405` Windows signatures changed since the latest version came out.
- `5/405` Linux signatures changed since the latest version came out.
4. `Pre-Current (6-15-2021)`
- `51/405` Windows signatures changed since the latest version came out.
5. `Pre-Current 2 (12-9-2021)`
- `17/405` Windows signatures changed since the latest version came out.
6. `Pre-Current 3 (2-1-2022)`
- `7/405` Windows signatures changed since the latest version came out.
7. `Current (4-14-2022)`

### Reminders
- Keep in mind that does not mean that most of these signatures will never break. It just means that they are durable enough to withstand several major updates unless VALVe updates the code of their respective functions and/or uses different compiler settings.

## Credits
Thank you to the following people for helping me locate a lot of these functions:
- **epz/epzminion**: Taught me everything about sigscanning, patching, vtable look-ups, etc.
- **Silvers (SilverShot)**: Leaves great notes in his gamedata files and also introduced the method of including the `CC ...` lines plus the first few bytes of following functions to create unique signatures for very short functions.
- **Lux/LuxLuma**: Uses lots of functions that are uncommonly used.
- **BHaType**: Uses lots of functions that are rarely used.
- **cravenge**: Uses some functions that are rarely used.
- **Scag/Scags**: Wrote several useful/helpful [IDA scripts](https://github.com/Scags/IDA-Scripts) to help make all of this a faster process.

## Other Resources
**[All Linux Signatures](https://github.com/dragokas/SM-Signatures)** by Dragokas - A repository for all the Linux signatures in the L4D/L4D2 binaries.

## Final Words
I hope that people can make use of all the signatures provided in this repository. I would appreciate if you could credit me (or whoever contributed) when using any of these signatures. I don't require any specific way of being credited so long as you mention my name and/or link this repository in your project information.
