# V6: Interaction with the environment

## Control objective

The controls in group this ensure that the app uses operation system APIs and standard components in a secure manner. Additionally, the controls cover communication between apps (IPC).

## Requirements

| # | Description | 1 | 2 | 3 | 4 |
| --- | --- | --- | --- | --- | --- |
| **6.1** | Verify that that the app does not request any unnecessary permissions. | ✓ | ✓ | ✓ | ✓ |
| **6.2** | Verify that all inputs from external sources is validated. This includes data reveived via the GUI, IPC mechanisms such as intents, custom URLs, and network communication.| ✓ | ✓ | ✓ | ✓ |
| **6.3** | Verify that the app does not export sensitive functionality via custom URL schemes. | ✓ | ✓ | ✓ | ✓ |
| **6.4** | Verify that the app does not export sensitive activities through intent filters (Android). | ✓ | ✓ | ✓ | ✓ |
| **6.5** | Verify that Javascript is disabled in all WebViews unless explicitly required. | ✓ | ✓ | ✓ | ✓ |
| **6.6** | Verify that file access is disabled in all WebViews unless explicitly required. | ✓ | ✓ | ✓ | ✓ |
| **6.7** | If Javascript is required in a WebView, ensure that the WebView is restricted to a specific URL, and that no unfiltered user input is rendered in the WebView. | ✓ | ✓ | ✓ | ✓ |
| **6.8** | Verify that the app provides a custom keyboard whenever sensitive data is entered. |   |   | ✓ | ✓ |
| **6.9** | Verify that custom ui-components are used when sensitive data is displayed. The UI-component should not rely on immutable data structures. |   |   | ✓ | ✓ |
| **6.10** | If Java objects are exposed in a WebView, verify that the WebView only renders JavaScript contained within the APK (Android). | ✓ | ✓ | ✓ | ✓ |
| **6.11** | Verify that the app updates the Security Provider if needed (Android). |   | ✓ | ✓ | ✓ |

## References

https://developer.android.com/training/articles/security-tips.html#IPC
https://developer.apple.com/library/content/documentation/iPhone/Conceptual/iPhoneOSProgrammingGuide/Inter-AppCommunication/Inter-AppCommunication.html
https://developer.android.com/reference/android/webkit/JavascriptInterface.html

For more information, please see:

(...) TODO - Link to MSTG (...)
