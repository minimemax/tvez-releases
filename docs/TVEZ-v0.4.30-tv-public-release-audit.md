# TVEZ 0.4.30-tv (Carmel) - Public Release Verification Summary

Report updated: 2026-09-24. Findings apply only to the APK identified below.

## APK identity

| Item | Value |
| --- | --- |
| File | `TVEZ-v0.4.30-tv.apk` |
| Package | `il.tvez.tv` |
| Version | `0.4.30-tv` (version code `43`) |
| Size | 15,089,953 bytes |
| Platform | Android TV; minimum API 23, target API 35 |
| SHA-256 | `1704be8fa582a2dd69cc78be93ca640a7f75ae54cfb2fa2752aefd70a8fe5a0b` |

Before installing, verify that the downloaded file's SHA-256 matches this value.

## Release signature

- Release build with R8 optimization and code obfuscation, plus resource shrinking; the release manifest is not debuggable.
- APK signature schemes v1, v2 and v3, and ZIP alignment, passed verification.
- Signing certificate SHA-256: `bdf80487ed585c446c5b8a5abd539401ee91809ab12b053f5459adf9fe93dba0`.
- Public-key SHA-256: `a218fe909d6d58ce00d0c7cc6326faa5404abdc1e41aa527580e957b516dc8e1`.
- Certificate subject: `CN=TVEZ Android TV Update, O=TVEZ, C=IL`.

The checksum identifies this exact binary. The verified signature confirms its integrity and continuity with the existing TVEZ signing certificate; it does not certify the app's behavior. R8 obfuscation makes code harder to inspect, but does not encrypt the package contents.

## External malware scans

| Service | Observed result | Report |
| --- | --- | --- |
| VirusTotal | 0 detections out of 65 engines; 1 timed out and 8 could not process the file type. | [View VirusTotal report](https://www.virustotal.com/gui/file/1704be8fa582a2dd69cc78be93ca640a7f75ae54cfb2fa2752aefd70a8fe5a0b) |

The VirusTotal report identifies the same SHA-256 as the APK above. These are point-in-time scan results, not a guarantee that the application is free of malware or vulnerabilities. Results may change after later scans.

## Requested permissions

| Permission | Declared purpose |
| --- | --- |
| `android.permission.INTERNET` | Network access for application services. |
| `android.permission.ACCESS_NETWORK_STATE` | Check network connectivity. |
| `android.permission.WAKE_LOCK` | Keep required playback or background work active. |
| `android.permission.RECEIVE_BOOT_COMPLETED` | Receive the system startup event for scheduled work. |
| `android.permission.FOREGROUND_SERVICE` | Run foreground services. |
| `android.permission.FOREGROUND_SERVICE_DATA_SYNC` | Identify foreground data-sync work. |
| `android.permission.FOREGROUND_SERVICE_MEDIA_PLAYBACK` | Identify foreground media-playback work. |
| `android.permission.POST_NOTIFICATIONS` | Post app notifications where supported. |
| `android.permission.SCHEDULE_EXACT_ALARM` | Schedule time-sensitive app tasks. |
| `android.permission.REQUEST_INSTALL_PACKAGES` | Request Android installation of optional channel shortcuts. |
| `android.permission.REQUEST_DELETE_PACKAGES` | Request Android removal of optional channel shortcuts. |
| `il.tvez.tv.permission.MANAGE_CHANNEL_SHORTCUTS` | App-defined permission for TVEZ channel-shortcut communication. |
| `com.android.providers.tv.permission.WRITE_EPG_DATA` | Write programme entries to the Android TV provider. |
| `com.android.providers.tv.permission.READ_EPG_DATA` | Read programme entries from the Android TV provider. |
| `il.tvez.tv.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION` | App-defined protection for internal runtime receivers. |

No camera, microphone, location, contacts, SMS or advertising-ID permission is declared. The manifest permission list alone is not a complete assessment of runtime data handling.

## Verification scope and limitations

- Release APK assembly and release lint checks passed.
- 794 automated unit tests passed; none failed or were skipped.
- APK package identity, version metadata, release signature and ZIP alignment passed local verification.
- This report does not claim emulator or physical-device runtime testing, a network-traffic audit, an independent security certification or a penetration test.
- External streams and programme-guide services may change independently of the application.

