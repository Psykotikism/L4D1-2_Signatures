# L4D1&2 Signatures

## About
This is a repository for hosting/storing several L4D1&2 signatures. More signatures will be added and supported as I come across or use more functions. I will try my best to keep all the signatures in this repository up-to-date.

- If you want me to add/support any function that isn't in this repository already, file an issue.
- If you have some signatures you want to share, make a pull request.

## Notes

### General
- Most of these signatures are designed for detours since that is the only reason I sought most them in the first place. You can of course still use them for `SDKCall`'s and/or `Addresses`.
- Keep in mind that most plugins that are still being maintained already use up-to-date signatures, so unless you are getting errors for any of these functions, you do not need to use any of these signatures.
- Most of these signatures are heavily wildcarded but have been tested across multiple versions of both games to be very durable. While shorter signatures are ideal, longer but durable ones are more convenient.

### Signature Count
- **L4D1**: 224
- **L4D2**: 304

### Left 4 Dead 2
- Most of the signatures have been verified to have withstood the last 5 landmark updates:
1. `Pre-TLS (6-5-2020)` - `28/304` changed since the latest version came out.
2. `TLS (9-24-2020)` - `23/304` changed since the latest version came out.
3. `Post-TLS (2-18-2021)` - `23/304` changed since the latest version came out.
4. `Post-Post-TLS (6-15-2021)` - `22/304` changed since the latest version came out.
5. `Current (7-8-2021)`
- Keep in mind that does not mean that most of these signatures will never break. It just means that they are durable enough to withstand several major updates unless VALVe updates the code of their respective functions and/or uses different compiler settings.

## Credits
Thank you to the following people for helping me locate a lot of these functions:
- **epz/epzminion**: Taught me everything about sigscanning, patching, vtable look-ups, etc.
- **Silvers (SilverShot)**: Leaves great notes in his gamedata files and also introduced the method of including the `CC ...` lines plus the first few bytes of following functions to create unique signatures for very short functions.
- **Lux/LuxLuma**: Uses lots of uncommon functions that no other person uses.
- **BHaType**: Uses lots of rare functions that no other person thinks to utilize.
- **Scag/Scags**: Wrote several useful/helpful IDA scripts to help make all of this a faster process.