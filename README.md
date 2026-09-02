# Castlevania: Aria of Sorrow - Italian Enhanced Edition

**English** · [Italiano](README.it.md)

Unofficial Italian Enhanced Edition of *Castlevania: Aria of Sorrow* for Game Boy Advance, with improved colours and optional gameplay adjustments.

## Included in every variant

- **[Italian translation v2.0](https://romhacking.it/project/view/id/190)** by Evrain.
- **[Colour Improvement v1.2](https://www.romhacking.net/hacks/9121/)** by Piggy Chan!, ported from the USA ROM to the European ROM.
- **[INT fix](https://www.romhacking.net/hacks/5645/)** by Dev Anj: Bullet souls correctly benefit from Soma's INT stat.
- **[LCK fix](https://www.romhacking.net/hacks/5645/)** by Dev Anj: LCK has a meaningful effect on item and soul drop rates.

Optional variants add:

- **[MP Regen](https://www.romhacking.net/hacks/5645/)** by Dev Anj: increases MP regeneration speed.
- **[Better Drops](https://github.com/Xanthus1/aos_patches)** by Xanthus: raises the base item and soul drop rates.

Every release patch is cumulative: apply one file directly to the clean European ROM. All variants already include the four components above.

## Variants

| Variant | Additional changes | Balance impact | Patch |
|---|---|---|---|
| Standard | None | Closest to the original balance | [`castlevania-aos-ita-v1.0.0.ips`](patches/castlevania-aos-ita-v1.0.0.ips) |
| MP Regen | Faster MP regeneration | Easier long fights, with souls available more often | [`castlevania-aos-ita-v1.0.0-mp.ips`](patches/castlevania-aos-ita-v1.0.0-mp.ips) |
| Better Drops | Higher base item and soul drop rates | Less farming | [`castlevania-aos-ita-v1.0.0-drop.ips`](patches/castlevania-aos-ita-v1.0.0-drop.ips) |
| Complete | MP Regen and Better Drops | Most forgiving, combining both advantages | [`castlevania-aos-ita-v1.0.0-mp-drop.ips`](patches/castlevania-aos-ita-v1.0.0-mp-drop.ips) |

MP Regen comes from the original Dev Anj archive. Better Drops uses the six optional drop-threshold changes from Xanthus's [LCK Plus Better Drop Rates](https://github.com/Xanthus1/aos_patches). These changes are not part of the standard LCK fix.

### Resulting ROM hashes

- Standard: `9300CC40EC53AB8C0C30067928E017163F836887198363B3DC7AAB0C12DEB630`
- MP Regen: `5DF1D21C383DF914274744F82CE8F1BDE880624CF308651705E6E8522E8C022B`
- Better Drops: `9308FAA239C38EF1FDCEBB7E41011443AB648AFC6C53C976FE36DF4AE5BF48B7`
- Complete: `3A4DE409EC8427AF86CAF10FE856F1A1B204D690899DEE69B300C959E2260A16`

## Required ROM

Apply the patch directly to a clean European ROM matching all of these values:

| Property | Expected value |
|---|---|
| Title | `Castlevania - Aria of Sorrow (Europe) (En,Fr,De)` |
| Game code | `A2CP` |
| CRC32 | `D0C91F74` |
| SHA-1 | `2E8302C2A5A61614749F609D7EDC8C3E6AF20585` |

Do not apply the patch to the USA ROM or to an already modified ROM.

## Installation

1. Verify that your ROM matches the hashes above.
2. Make a backup of the original file.
3. Choose one variant from the table and apply that IPS with [Lunar IPS](https://fusoya.eludevisibility.org/lips/) or another IPS-compatible patcher.
4. Start the resulting ROM in your preferred emulator or compatible hardware.

Compare the resulting ROM with the SHA-256 listed for the selected variant.

## Verification

Each patch produces the ROM hash listed in the variants table.

INT and LCK were checked with focused emulator tests. The standard variant also completed both phases of the Chaos battle and ran through frame 20,001 without crashing. The MP and Complete variants passed startup smoke tests.

Testing covered the modified systems and one late-game sequence, not a complete playthrough.

## Credits

- **Evrain:** Italian translation v2.0.
- **OldHouse, IKKI_THE_FENIX and Il Pulciaro:** original translation beta testing.
- **_Scorpio_:** ROM-hacking assistance for the original translation.
- **Brisma:** GBA pointer information for the original translation.
- **Clomax and Tidus:** special thanks in the original translation readme.
- **Piggy Chan!:** Colour Improvement v1.2.
- **Dev Anj:** original INT, LCK and MP Regen patches.
- **Rabite:** documentation and authorized publication of Dev Anj's patches.
- **Xanthus:** optional Better Drops modifications.
- **Bruc3Dev573:** European integration, patch preparation and verification.

Dev Anj's redistribution permission and original description are preserved verbatim in [`docs/DevAnj-LCKFix-license-readme.txt`](docs/DevAnj-LCKFix-license-readme.txt).

Attribution and redistribution terms for original project material are in [`NOTICE`](NOTICE).

## Legal notice

This is an unofficial, non-commercial fan project. Konami and the original authors are not involved with it. The repository contains patches, checksums and documentation only. It does not contain ROMs or save data.

You must own a legitimate copy of the game. Rights holders and original authors may request corrections, attribution changes or removal through GitHub Issues.
