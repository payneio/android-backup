# android-backup

Back up an Android device over ADB (Android Debug Bridge).

Backs up photos, videos, documents, app data, SMS, RCS, contacts, and call logs
from any Android device that supports ADB. Requires `adb` installed and the
device connected with USB debugging enabled.

## Usage

```bash
android-backup                      # Back up using the default configuration
android-backup -c custom.json       # Use a custom configuration file
android-backup --photos-only        # Only back up photos
android-backup --sms-only           # Only back up SMS messages
android-backup --contacts-only      # Only back up contacts
android-backup --app-data whatsapp  # Only back up a specific app's data
android-backup --device serialnum   # Pick a device when several are connected
```

## Install

```bash
uv tool install --editable .
```

## License

Copyright (C) 2026 Paul Payne. Licensed under the GNU AGPLv3 — see [LICENSE](LICENSE).
