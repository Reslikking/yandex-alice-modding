# Yandex Station Mini 2 — Technical Profile

## 1. Overview

This document describes the tested Yandex Station Mini 2 device, its documented hardware characteristics, baseline test results, and the current state of community research into diagnostics and system modification.

The project distinguishes between:
- **Verified:** directly observed on the test device or documented by an official source.
- **Reported:** claimed by an independent community project but not independently reproduced here.
- **Unknown:** not yet tested or confirmed.

A result obtained on one firmware build must not be assumed to apply to another build.

## 2. Test Device

| Property | Value | Status |
|---|---|---|
| Product | Yandex Station Mini 2 with clock display | Verified |
| Model number | `YNDX-00020` | Verified |
| Firmware | `0.369.1.50.4794659041.20261021.299` | Verified |
| Baseline test date | 2026-10-27 | Verified |
| App device name | `Станция Мини new` | Verified |
| Clock display | Present | Verified |
| Alice animation | Observed during baseline testing | Verified |
| Account ownership | Device currently linked to a family member's account | Verified |
| Root access | Not tested | Unknown |
| ADB access | Not tested | Unknown |
| Bootloader or recovery access | Not tested | Unknown |
| Firmware downgrade compatibility | Not verified for this project | Unknown |

Private device identifiers, account details, network addresses, credentials, and tokens are intentionally excluded.

## 3. Official Hardware Specifications

The following specifications are published by Yandex for Station Mini 2.

| Component | Official specification |
|---|---|
| Speaker | One 10 W full-range speaker |
| Microphones | Four |
| Wireless networking | Wi-Fi 802.11 b/g/n/ac, 2.4 GHz and 5 GHz |
| Bluetooth | Bluetooth 5.0 and BLE |
| Display | Monochrome LED display on model YNDX-00020 |
| Display elements | 32 white LEDs |
| Audio output | AUX OUT |
| Power input | 15 V, 1.2 A nominal adapter output |
| Built-in battery | None |
| Water and dust protection | Not specified as protected |

Official documentation:
- [Station Mini 2 specifications](https://alice.yandex.ru/support/ru/station/meet/characteristics-mini2)
- [Identify your Yandex Station model](https://alice.yandex.ru/support/ru/station/identify.html)
- [Station Mini 2 help](https://alice.yandex.ru/support/ru/station/index-mini2)

These are product-level specifications. They do not establish the internal SoC, RAM, storage layout, boot chain, operating system version, or security configuration of this particular unit.

## 4. Baseline Functionality

The following tests were performed on 2026-10-27 using firmware `0.369.1.50.4794659041.20261021.299`.

| Test | Result |
|---|---|
| Normal startup | PASS |
| Alice voice responses | PASS |
| Clock display and Alice animation | PASS |
| Wi-Fi connectivity | PASS |
| Music playback | PASS |

No system modifications were performed during baseline testing.

These results confirm basic operation only. They do not establish root access, ADB availability, firmware downgrade support, or the ability to disable automatic updates.

## 5. Firmware and Compatibility

### Tested firmware

`0.369.1.50.4794659041.20261021.299`

This is the firmware observed on the test device during baseline testing.

### Community-reported compatibility

The independent project [hu553in/yandex-station-root](https://github.com/hu553in/yandex-station-root) reports testing its root ADB method on Station Mini 2 model `YNDX-00020` with firmware:

`0.369.1.46.4778262943.20261013.299`

The project's compatibility note states that the `.50` firmware build rejects the certificate authority chain used by that method.

These are third-party claims, not results reproduced by this repository.

**Current conclusion:** the root ADB method must be treated as incompatible or unverified on the test firmware until a safe, independently reproducible test establishes otherwise. Successful operation on `.46` does not prove compatibility with `.50`.

## 6. Root and ADB Research Status

| Capability | Status | Notes |
|---|---|---|
| Normal user functionality | Verified | Baseline tests passed |
| ADB availability | Unknown | No connection attempt performed |
| Root privileges | Unknown | No root test performed |
| Persistent ADB after reboot | Unknown | Not tested |
| Firmware downgrade | Unknown | No downgrade performed |
| OTA update control | Unknown | No update settings modified |
| Recovery procedure for modified firmware | Not established | No modification has been attempted |

No root exploit, certificate interception, DNS override, firmware downgrade, or system-file modification has been performed by this project.

### Important limitations

- Community instructions may depend on the exact firmware build.
- A platform profile or firmware archive does not prove that a procedure works.
- Firmware downgrade can fail or leave the device unusable.
- Persistent network ADB can expose privileged access to other devices on the local network.
- Disabling automatic updates can reduce security and complicate recovery.
- Backups and recovery instructions must be verified before any future modification.

## 7. Account and Ownership Constraints

The test device is currently linked to a family member's Yandex account.

Before attempting any reset, reconfiguration, firmware modification, or account-related operation, obtain the account owner's permission. Avoid steps that could remove the device from its current account or disrupt normal household use.

## 8. Next Research Tasks

1. Preserve the baseline test report and firmware version.
2. Review official documentation and independent technical sources.
3. Record any new observations with the exact firmware version and test conditions.
4. Determine whether supported, non-destructive diagnostic interfaces exist for this model.
5. Assess recovery options before considering system modifications.
6. Independently verify every claimed result before marking it as confirmed.

Any future experiment should have its own report containing the objective, prerequisites, exact device firmware, procedure, expected outcome, actual result, risks, and recovery status.

## 9. Safety and Privacy

- Do not commit account tokens, passwords, private device IDs, Wi-Fi credentials, or other secrets.
- Do not publish unredacted diagnostic logs containing personal or network information.
- Do not treat an AI-generated explanation or a community post as proof of compatibility.
- Keep original files and verified backups if authorized modifications are eventually undertaken.
- Do not label a procedure as safe or reproducible until it has been tested and its recovery path documented.

## 10. Disclaimer

This repository documents independent research and testing by Reslik king. It is not affiliated with, endorsed by, or supported by Yandex.

All third-party methods and compatibility claims are attributed to their respective sources. No claim of root access or firmware modification is made for the test device unless explicitly documented in a separate, reproducible test report.
No test result should be marked as verified until it has been reproduced and documented.
