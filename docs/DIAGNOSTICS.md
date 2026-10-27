# Yandex Station Diagnostics

## Scope
This document records official diagnostic information and separates confirmed facts from unverified research.

## Test Device
- Model: YNDX-00020
- Device name in app: Станция Мини new
- Firmware: `0.369.1.50.4794659041.20261021.299`
- Baseline functionality: Passed all five checks on 2026-10-27

## Official Information
- [Station Mini 2 — official help](https://alice.yandex.ru/support/ru/station/index-mini2)
- [Station Mini 2 specifications](https://alice.yandex.ru/support/ru/station/meet/characteristics-mini2)
- [Identify your Station model](https://alice.yandex.ru/support/ru/station/identify.html)
- [Firmware update information](https://alice.yandex.ru/support/ru/station/settings/update)

## Confirmed
- The device reports model number YNDX-00020.
- The app reports firmware `0.369.1.50.4794659041.20261021.299`.
- Startup, voice responses, clock animation, Wi-Fi, and music playback passed baseline checks.

## Not Yet Verified
- A public community project reports testing root ADB on firmware `0.369.1.46.4778262943.20261013.299`.
- The same project reports that firmware `0.369.1.50.4794659041.20261021.299` rejects the certificate chain used by its method.
- These reports have not been independently reproduced for this project.
- Compatibility with this device's exact firmware remains unverified.
- No DNS changes, certificate interception, or system modifications have been performed.
- The Yandex Station Extended community wiki documents an AliceBridge method for obtaining root through Android.
- As of 2026-10-25, the wiki lists Yandex Station Mini 2 as requiring verification for its firmware profile.
- Availability of a firmware profile does not confirm successful root access on this device.
- Source: https://hackalice.me/start/root-android/
- Source: https://hackalice.me/devices/yandexmini_2/

## Safety and Reproducibility
- Do not publish device identifiers, account details, Wi-Fi credentials, or tokens.
- Do not change router DNS or reset the device during baseline documentation.
- Record firmware version, test date, exact steps, outcome, and recovery method for each experiment.
- Mark a result as verified only after reproducing it.

## Disclaimer
Independent community research by Reslik king. Not affiliated with or endorsed by Yandex.
