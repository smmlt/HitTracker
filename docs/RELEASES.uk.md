# Android-релізи

[English](RELEASES.md) · **Українська**

Усі APK-файли опубліковано в [GitHub Releases](https://github.com/smmlt/hit-tracker-mobile/releases). Остання стабільна збірка завжди доступна за [посиланням на актуальний реліз](https://github.com/smmlt/hit-tracker-mobile/releases/latest).

| Реліз | Тип APK | Основні зміни | SHA-256 |
|---|---|---|---|
| [v1.1.2 · Build 10](https://github.com/smmlt/hit-tracker-mobile/releases/tag/android-v1.1.2-build10) | Universal | Прокручувані вкладки адмінпанелі на вузьких екранах, Android 7+, чотири ABI | `D5924CE7A29E8B12F89BCD0D633167E68E23D3A2E439CBA18A909C3393FFF6DA` |
| [v1.0.2 · Build 4](https://github.com/smmlt/hit-tracker-mobile/releases/tag/android-v1.0.2-build4) | Universal | Фірмовий splash screen, центрована іконка, Android 7+, чотири ABI та постійний ключ підпису | `566C3294C4C736F4C66EBEC8C6F22E4FE56AB79364D80E1351706B1C8AD19E77` |
| [v1.0.1 · Build 3](https://github.com/smmlt/hit-tracker-mobile/releases/tag/android-v1.0.1-build3) | ARM64 | Фірмова іконка застосунку та виправлення нативного завантаження фотографії профілю | `4E2FE783D9CDECE62A4428659349A1C9E5D67FCF0157085C2EFCD71004FBC583` |
| [v1.0.0 · Build 2](https://github.com/smmlt/hit-tracker-mobile/releases/tag/android-v1.0.0-build2) | ARM64 | Перша локальна Gradle-збірка та виправлення Android safe area | `D3F59328613FF39564D7857245064F65CE2171A6ED0F862EC0033357CBFB66AA` |
| [v1.0.0 · Build 1](https://github.com/smmlt/hit-tracker-mobile/releases/tag/android-v1.0.0-build1) | Universal | Перша Android-збірка через Expo/EAS | `DADB60323208EF72501967C017583329B90151E7C85FB51B51CCC02C59C47D5F` |

## Перехід на постійний підпис

Build 1–3 створено з попередніми тестовими або хмарними обліковими даними. У Build 4 уперше використано постійний release-сертифікат HitTracker:

```text
SHA-256: 8D400F4DD29A984152E0A15F6C8DB96032F73A59E3665B6B41CAC185A1020132
Subject: CN=HitTracker
Algorithm: RSA 4096
```

Android приймає оновлення поверх установленої версії лише тоді, коли підписи встановленого та нового пакетів сумісні. Один раз видаліть Build 1–3 перед установленням Build 4. Наступні збірки, підписані постійним ключем, зможуть оновлювати Build 4 звичайним способом.
