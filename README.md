# desktop_webview_window

## Original Project
- [pub.dev/packages/desktop_webview_window](https://pub.dev/packages/desktop_webview_window)
- [MixinNetwork/flutter-plugins-desktop_webview_window](https://github.com/MixinNetwork/flutter-plugins/tree/main/packages/desktop_webview_window)

## Change Log
- support: GetAllCookies
```dart
import 'package:desktop_webview_window/desktop_webview_window.dart';

void main() async {
    final webview = await WebviewWindow.create();
    webview.launch("https://github.com");
    await Future.delayed(const Duration(seconds: 5));

    /// print all cookies String - only Windows
    /// return example: logged_in=no; preferred_color_mode=dark; tz=Asia%2FShanghai
    print(await webview.getAllCookies());
}
```

## License
Apache License
