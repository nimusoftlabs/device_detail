A library for getting platform information.


This lightweight package allows in a very simple and optimized way to obtain Info about the platform on which it is running. It's multi-platform, and supports mobile, desktop,
and the browser.

## Using

The easiest way to use this library is to call the class as follows. 
Multiple instances are not being created since thanks to a factory constructor it always 
returns an internal singleton:

```dart
import 'package:device_detail/device_detail.dart';

if (DeviceDetail().isMobile) {
  print('The current platform is Mobile');
}  

if (DeviceDetail().isDesktopOrWeb) {
  print('The current platform is Desktop or Web');
}

if (DeviceDetail().isDesktop) {
  print('The current platform is Desktop');
}

if (DeviceDetail().isWeb) {
  print('The current platform is web');
}
```

If instead you want to ask individually for each platform supported by Flutter:

```dart
if (DeviceDetail().isIOS) {
  print('The current platform is iOS');
}

if (DeviceDetail().isAndroid) {
  print('The current platform is Android');
}

if (DeviceDetail().isFuchsia) {
  print('The current platform is Fuchsia');
}

if (DeviceDetail().isWindows) {
  print('The current platform is Windows');
}

if (DeviceDetail().isLinux) {
  print('The current platform is Linux');
}

if (DeviceDetail().isMacOS) {
  print('The current platform is macOS');
}
```