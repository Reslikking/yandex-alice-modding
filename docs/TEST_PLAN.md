# Yandex Alice — Practical Test Plan

## 1. Objective

Define a repeatable process for testing Yandex Alice smart speaker functionality.

## 2. Test Preconditions

- Record the exact device model.
- Record the firmware version.
- Confirm that the device is connected to its normal network.
- Confirm that the official application detects the device.
- Obtain the device owner's permission before testing.

## 3. Basic Functionality Tests

- Verify normal startup.
- Test voice activation.
- Test a basic voice command.
- Test music playback using an officially supported service.
- Test volume adjustment.
- Test normal restart and recovery.

## 4. Test Results

For each test, record:

- Test date
- Device model and firmware
- Steps performed
- Expected result
- Actual result
- Pass, fail, or not tested
- Notes and evidence

## 5. Safety

- Do not attempt to bypass authentication or access controls.
- Do not publish passwords, tokens, or private device information.
- Do not modify firmware until a documented recovery procedure is available.

## 6. Current Status

Status: Basic functionality tests passed on 2026-10-27. ADB research has not started.

## ADB Research — YNDX-00020

### Objective
Determine what is publicly documented about ADB availability on the recorded firmware.

### Current Status
- Firmware recorded: `0.369.1.50.4794659041.20261021.299`
- ADB availability: Unknown
- ADB authentication requirements: Unknown
- Root access: Not tested
- System modifications: None

### Research Procedure
1. Review publicly available documentation for the exact device model and firmware.
2. Separate reports for other firmware versions from evidence for this build.
3. Prefer documented diagnostic methods that do not change device or router settings.
4. Record the source, date, procedure, and limitations of each finding.
5. Do not claim ADB or root access is available without reproducible evidence.

### Success Criteria
A finding is considered confirmed only when its source and test conditions are documented and the result is reproducible.

### Safety
Do not expose device identifiers, account credentials, authentication tokens, or Wi-Fi passwords.
