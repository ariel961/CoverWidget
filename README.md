# Cover Widget for Galaxy Z Fold

Shows unread WhatsApp, Gmail and Outlook counts, your next alarm, battery %, and a Sound/Silent button.

## Build and install (about 20 minutes)

1. Install Android Studio (developer.android.com/studio) on a computer.
2. Unzip this folder, then in Android Studio choose File > Open and pick the CoverWidget folder.
   Wait for Gradle sync to finish (the first time can take several minutes). If it offers to
   upgrade the Android Gradle Plugin, accepting is fine.
3. On the phone: Settings > About phone > Software information, tap "Build number" 7 times.
   Then Settings > Developer options > turn on USB debugging.
4. Connect the phone by USB and allow debugging when the phone asks.
5. In Android Studio, pick your phone in the device menu at the top and press the green Run button.

## Set up on the phone

1. The Cover Widget setup screen opens. Tap "Grant notification access" and switch Cover Widget on.
   This usually also allows Silent mode. If the status still shows ✗ for silent, tap "Allow silent mode".
2. Close the phone, long-press an empty spot on the cover screen, tap Widgets, find Cover Widget, drag it on.
3. Resize it by long-pressing the widget and dragging the edges.

## How it behaves

- Unread counts come from notifications. Reading a message elsewhere or swiping its
  notification away lowers the count. Gmail and Outlook only count accounts and folders
  you have notifications turned on for.
- Tap a row to open that app. Tap the alarm to open the Clock app. Tap the battery to open battery settings.
- Battery % turns red at 15% or below and shows a lightning bolt while charging.
- Android only shares the next alarm, so after one rings the widget shows the other.
- Samsung may pause background apps to save battery. If counts stop updating, go to
  Settings > Battery > Background usage limits and add Cover Widget to "Never sleeping apps".

## Customize

- Different apps: edit package names in Apps.kt (WhatsApp Business is com.whatsapp.w4b).
- Colors: res/values/colors.xml (light) and res/values-night/colors.xml (dark).
