# Android releases

**English** · [Українська](RELEASES.uk.md)

All APK files are published through [GitHub Releases](https://github.com/smmlt/hit-tracker-mobile/releases). The latest stable build is always available at the [latest-release link](https://github.com/smmlt/hit-tracker-mobile/releases/latest).

| Release | APK type | Main changes | SHA-256 |
|---|---|---|---|
| [v1.1.2 · Build 10](https://github.com/smmlt/hit-tracker-mobile/releases/tag/android-v1.1.2-build10) | Universal | Scrollable admin tabs on narrow screens, Android 7+, four ABIs | `D5924CE7A29E8B12F89BCD0D633167E68E23D3A2E439CBA18A909C3393FFF6DA` |
| [v1.0.2 · Build 4](https://github.com/smmlt/hit-tracker-mobile/releases/tag/android-v1.0.2-build4) | Universal | Branded splash, centered icon, Android 7+, four ABIs, permanent signing key | `566C3294C4C736F4C66EBEC8C6F22E4FE56AB79364D80E1351706B1C8AD19E77` |
| [v1.0.1 · Build 3](https://github.com/smmlt/hit-tracker-mobile/releases/tag/android-v1.0.1-build3) | ARM64 | Branded launcher icon and native profile-photo upload fix | `4E2FE783D9CDECE62A4428659349A1C9E5D67FCF0157085C2EFCD71004FBC583` |
| [v1.0.0 · Build 2](https://github.com/smmlt/hit-tracker-mobile/releases/tag/android-v1.0.0-build2) | ARM64 | First local Gradle build and Android safe-area fixes | `D3F59328613FF39564D7857245064F65CE2171A6ED0F862EC0033357CBFB66AA` |
| [v1.0.0 · Build 1](https://github.com/smmlt/hit-tracker-mobile/releases/tag/android-v1.0.0-build1) | Universal | First Expo/EAS Android build | `DADB60323208EF72501967C017583329B90151E7C85FB51B51CCC02C59C47D5F` |

## Signing transition

Builds 1–3 were created with earlier test or cloud credentials. Build 4 introduced the permanent HitTracker release certificate:

```text
SHA-256: 8D400F4DD29A984152E0A15F6C8DB96032F73A59E3665B6B41CAC185A1020132
Subject: CN=HitTracker
Algorithm: RSA 4096
```

Android only accepts an in-place update when the installed and incoming packages have compatible signatures. Remove a Build 1–3 installation once before installing Build 4. Builds signed with the permanent key can then update Build 4 normally.
