# TVEZ 0.4.31-tv (Carmel) - Public Release Audit

Updated: 2026-09-24

## Release artifact

| Item | Value |
| --- | --- |
| File | `TVEZ-v0.4.31-tv.apk` |
| Version | `0.4.31-tv` (version code `44`) |
| Package | `il.tvez.tv` |
| Android API | Minimum `23`; target `35` |
| File size | `15,089,953` bytes |
| SHA-256 | `551174bf4a15e34de32dffffcd4fc3db3db9bb89450f0d8c36967dc73273ba56` |

## Release integrity

- Release build uses R8 optimization and code obfuscation, with resource shrinking enabled. The R8 mapping was generated for the matching release build, and the signed APK payload matches that build.
- The release manifest is not debuggable.
- APK signature schemes v1, v2 and v3, and ZIP alignment, passed verification.
- Signing certificate SHA-256: `bdf80487ed585c446c5b8a5abd539401ee91809ab12b053f5459adf9fe93dba0`.
- Public-key SHA-256: `a218fe909d6d58ce00d0c7cc6326faa5404abdc1e41aa527580e957b516dc8e1`.
- Certificate subject: `CN=TVEZ Android TV Update, O=TVEZ, C=IL`.

The checksum identifies this exact APK. The verified signature confirms integrity and continuity with the TVEZ signing certificate; it does not certify the app's behavior. R8 obfuscation makes code harder to inspect, but does not encrypt the package contents.

## VirusTotal

At the time of the displayed analysis on 2026-09-24, 0 of 65 security vendors flagged the file. A few engines timed out or did not support the file type, so this result is not a guarantee of safety.

[View the VirusTotal report for this SHA-256](https://www.virustotal.com/gui/file/551174bf4a15e34de32dffffcd4fc3db3db9bb89450f0d8c36967dc73273ba56)

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

No camera, microphone, location, contacts, SMS or advertising-ID permission is declared. The permission list alone is not a complete assessment of runtime data handling.
