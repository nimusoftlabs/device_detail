A library for getting platform information.


This lightweight package allows in a very simple and optimized way to obtain Info about the platform on which it is running. It's multi-platform, and supports mobile, desktop,
and the browser.

## Using

The easiest way to use this library is to call the class as follows. 
Multiple instances are not being created since thanks to a factory constructor it always 
returns an internal singleton:

```dart
import 'package:device_info/device_info.dart';

if (PlatformInfo().isMobile) {
  print('The current platform is Mobile');
}  

if (PlatformInfo().isDesktopOrWeb) {
  print('The current platform is Desktop or Web');
}

if (PlatformInfo().isDesktop) {
  print('The current platform is Desktop');
}

if (PlatformInfo().isWeb) {
  print('The current platform is web');
}
```

If instead you want to ask individually for each platform supported by Flutter:

```dart
if (PlatformInfo().isIOS) {
  print('The current platform is iOS');
}

if (PlatformInfo().isAndroid) {
  print('The current platform is Android');
}

if (PlatformInfo().isFuchsia) {
  print('The current platform is Fuchsia');
}

if (PlatformInfo().isWindows) {
  print('The current platform is Windows');
}

if (PlatformInfo().isLinux) {
  print('The current platform is Linux');
}

if (PlatformInfo().isMacOS) {
  print('The current platform is macOS');
}
```