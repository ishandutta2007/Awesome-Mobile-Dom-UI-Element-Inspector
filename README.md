# Awesome-Mobile-Dom-UI-Element-Inspector

# Awesome Mobile DOM & UI Element Inspector

> A curated list of top Mobile DOM and UI Element Inspector platforms — both SaaS/Hosted commercial testing suites and open-source alternatives for inspecting view hierarchies, finding element locators, and debugging mobile app interfaces.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [BrowserStack Inspector](#browserstack-inspector)
  - [Appium Inspector](#appium-inspector)
  - [Safari Web Inspector](#safari-web-inspector)
  - [Android UI Automator Viewer](#android-ui-automator-viewer)
- [Open-Source Software](#-open-source-software)
  - [UiHound](#uihound)
  - [ViewScope](#viewscope)
  - [uiautodev](#uiautodev)
  - [ui-finder](#ui-finder)
  - [Smart XPath Locator](#smart-xpath-locator)
  - [Treescope](#treescope)
  - [hm-ui-viewer](#hm-ui-viewer)
  - [react-native-element-inspector](#react-native-element-inspector)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Mobile DOM and UI Element Inspector platforms. These are not open-source but are included as reference points for feature comparison.

### BrowserStack Inspector
**Type:** Cloud-based mobile app and web element inspection
BrowserStack provides interactive inspection capabilities within its real-device cloud, allowing teams to inspect DOM elements, view hierarchies, and debug mobile web and native app interfaces remotely. It is the natural choice for teams already using BrowserStack for cross-browser and mobile testing.

### Appium Inspector
**Type:** GUI inspector for Appium sessions
Appium Inspector is the official GUI tool for inspecting mobile app elements during Appium sessions, displaying the view hierarchy, element attributes, and locator suggestions. It is the standard companion tool for Appium automation, with a standalone desktop application available for macOS, Windows, and Linux [citation:9].

### Safari Web Inspector
**Type:** WebKit-based inspection for iOS and macOS
Safari Web Inspector provides DOM, CSS, and JavaScript debugging for web content in Safari and iOS WebViews. It is the native inspection tool for Apple platforms, requiring a Mac for full iOS device inspection.

### Android UI Automator Viewer
**Type:** Legacy Android view hierarchy inspector
UI Automator Viewer was a standalone tool in the Android SDK for inspecting view hierarchies and generating uiautomator locators. It has been deprecated in favor of newer tools like Appium Inspector and Layout Inspector, but remains referenced in older workflows.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Mobile DOM and UI Element Inspector tools. The open-source ecosystem spans **Android UI inspection web tools**, **cross-platform inspectors with code generation**, **iOS view tree inspectors**, and **in-app React Native element inspectors**.

### UiHound
**Stack:** Python / FastAPI / Web UI | **License:** Open Source (PyPI)
UiHound is a local web tool for Android debugging and UI automation, providing element inspection, locator finding, remote device control, and screenshot/recording capture [citation:2][citation:10]. Key capabilities include:
- **Element inspection**: Browse the UI hierarchy, view element properties, coordinates, and screen highlights
- **Locator finding**: Search for and copy u2 selectors or XPath expressions, prioritizing unique attributes
- **Remote control**: scrcpy-based live screen with taps, swipes, long presses, and navigation buttons
- **Color sampling**: Pixel magnifier with HEX, RGB, HSB, and OpenCV HSV values
- **Screenshot and recording**: Full-screen, element, and region screenshots plus WebM recording
- **Offline analysis**: Import an image and UI XML to inspect without a connected device

It runs locally at `http://127.0.0.1:8000` after `pip install uihound` [citation:2].
**Best for:** Android developers and QA engineers wanting a local, feature-rich UI inspector with remote control and locator generation, accepting the Python/ADB setup.

### ViewScope
**Stack:** Vue.js 3 / FastAPI / Python | **License:** MIT
ViewScope is a modern Android UI element inspector similar to weditor, built with Vue.js 3 and FastAPI [citation:3]. Key features include:
- **Device management**: Auto-detect and manage Android devices via ADB
- **Real-time screenshots**: High-quality PNG capture with an interactive SVG layer
- **Element selection**: Click any UI element to view details in the right panel
- **Code generation**: Auto-generate uiautomator2 locator code with one-click copy
- **UI hierarchy view**: Complete tree structure with search functionality
- **Multiple locator strategies**: Resource-ID, text, XPath, and more

It launches with `pip install ViewScope` and `viewscope`, starting a backend on port 8060+ and opening a browser interface [citation:3].
**Best for:** Android automation engineers wanting a modern web-based inspector with uiautomator2 code generation, accepting the Python/ADB dependency.

### uiautodev
**Stack:** Python / Prebuilt server binary | **License:** Open Source (PyPI)
uiautodev is a UI Inspector for **Android, iOS, and Harmony**, providing element property inspection and auto-generated XPath and scripts [citation:6]. Key characteristics:
- **Multi-platform support**: Android, iOS, and HarmonyOS
- **Prebuilt server binary**: `uiauto.dev` downloads a cached server binary and opens a browser interface
- **Offline mode**: `uiautodev server --offline` caches all frontend resources for use without internet
- **Driver options**: Defaults to uiautomator2, with an ADB driver alternative via environment variable

It is positioned as a cross-platform alternative to platform-specific inspectors [citation:6].
**Best for:** Teams needing a single inspector for Android, iOS, and HarmonyOS, accepting the prebuilt binary distribution model.

### ui-finder
**Stack:** Python / matplotlib / pyperclip | **License:** Open Source (PyPI)
ui-finder is a plug-and-play Python-based visual tool for inspecting Android app UI directly from a phone [citation:5]. Key features include:
- **Zero setup**: Auto-installs ADB and Python dependencies on first run
- **Live inspection**: Screenshot + hierarchy dump with click-to-highlight element selection
- **Dropdown filters**: Filter by class, resource-id, text, or bounds
- **One-click copy**: Copy element details to clipboard
- **Overlap handling**: Press `n` to cycle overlapping elements
- **Cross-platform**: Windows, Linux, and macOS

It installs via `pip install ui_finder` and runs offline after the first execution [citation:5].
**Best for:** Developers wanting a truly plug-and-play Android inspector that auto-installs its dependencies, accepting a simpler feature set than UiHound or ViewScope.

### Smart XPath Locator
**Stack:** Windows executable (likely .NET) | **License:** MIT
Smart XPath Locator is an advanced Android XML layout inspector and interactive XPath generator for Windows [citation:1]. Key features include:
- **Live device sync**: Connect via USB, Ethernet, or wireless ADB to inspect element hierarchies in real-time
- **Interactive canvas**: Click elements on a screenshot to highlight boundaries and load properties
- **XPath generation**: Copy optimized locators with one click
- **Excel export**: Generate spreadsheets containing element boundaries and cropped image snips
- **Offline inspection**: Load local screenshot and XML/UIX files

It is distributed as a Windows installer (`SmartXPathLocator_Setup.exe`) [citation:1].
**Best for:** Windows-based Android QA teams wanting a desktop inspector with Excel export capabilities, accepting the Windows-only limitation.

### Treescope
**Stack:** Swift / TypeScript / Browser viewer | **License:** MIT
Treescope is an open-source runtime view inspector for **UIKit, AppKit, and SwiftUI**, viewed in a browser [citation:8]. Key characteristics:
- **First-class SwiftUI inspection**: Opens `any View`, unwraps `ModifiedContent`, `TupleView`, and `_ConditionalContent`, reads `@State` and modifiers
- **Zero-install viewer**: The inspected app hosts the viewer itself over loopback HTTP at `http://127.0.0.1:50067`
- **3D exploded view**: Visualize layer hierarchies in an exploded 3D view
- **Live property editing**: Modify some properties live
- **No external dependencies**: Uses only `Network.framework` and `CryptoKit` for the embedded server

It is positioned as a free, open alternative to Lookin with first-class SwiftUI support [citation:8].
**Best for:** iOS and macOS developers wanting a zero-install, browser-based view inspector with full SwiftUI support, accepting that it requires embedding the debug server in the app.

### hm-ui-viewer
**Stack:** Python / FastAPI / Web UI | **License:** Open Source (PyPI)
hm-ui-viewer is a multi-platform UI layout viewer supporting **HarmonyOS and Android**, with a browser-based interface [citation:12]. Key features include:
- **Dual-pane layout**: Screenshot on the left with element borders, collapsible control tree on the right
- **Click linkage**: Clicking either the screenshot or tree node highlights the corresponding control
- **XPath generation**: Automatically generates multiple candidate XPaths sorted by stability
- **Offline file mode**: Upload screenshots and layout files for inspection
- **Desktop window mode**: Uses pywebview for a native window without a browser
- **Search**: Filter control nodes by type, text, or key

It requires Python 3.8+ with optional `hdc` (HarmonyOS) or `adb` (Android) for live device inspection [citation:12].
**Best for:** Teams working with both HarmonyOS and Android wanting a unified inspector, accepting the Python/FastAPI stack.

### react-native-element-inspector
**Stack:** React Native / TypeScript | **License:** Open Source (npm)
react-native-element-inspector is an **on-device element inspector for React Native**, providing an "Inspect Element" experience directly within the app [citation:13]. Key features include:
- **Tap to select**: Tap any element to inspect its styles, with overlapping elements sorted smallest-first
- **Live editing**: Edit style values inline, with changes applied instantly via React's reconciler
- **Property toggling**: Enable/disable properties without deleting them
- **Box model highlight**: Chrome DevTools-style overlay showing margin, padding, and content areas
- **Source mapping**: Displays component name and source file location
- **Zero native dependencies**: Pure TypeScript, works with React 18 and 19, Old Architecture and Fabric

Wrap the root component with `<ElementInspector enabled={__DEV__}>` to enable [citation:13].
**Best for:** React Native developers wanting an in-app inspector during development without external tools, accepting the React Native-specific scope.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Platform | Locator Generation | Live Device | Best For |
|----------|---------|-------|----------|---------------------|-------------|----------|
| **BrowserStack** | Proprietary | Cloud | Web + Native | (Check) | ✅ | BrowserStack users |
| **Appium Inspector** | Proprietary | Desktop | Android/iOS | ✅ | ✅ (Appium) | Appium automation |
| **UiHound** | Open Source | Python/FastAPI | Android | ✅ u2/XPath | ✅ | Local Android inspection + control |
| **ViewScope** | MIT | Vue/FastAPI | Android | ✅ uiautomator2 | ✅ | Web-based Android inspector |
| **uiautodev** | Open Source | Python/Binary | Android/iOS/Harmony | ✅ XPath | ✅ | Cross-platform inspection |
| **ui-finder** | Open Source | Python | Android | ✅ | ✅ | Plug-and-play Android inspector |
| **Smart XPath Locator** | MIT | Windows exe | Android | ✅ XPath | ✅ | Windows desktop + Excel export |
| **Treescope** | MIT | Swift/TS | iOS/macOS | ❌ | ✅ (Embedded) | SwiftUI view inspection |
| **hm-ui-viewer** | Open Source | Python/FastAPI | Android/Harmony | ✅ XPath | ✅ | Multi-platform (Harmony + Android) |
| **react-native-element-inspector** | Open Source | React Native | iOS/Android | ❌ (Styles) | ✅ (In-app) | In-app React Native debugging |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Mobile DOM or UI Element Inspector tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source.

**Note on the open-source ecosystem:** The mobile UI inspection space is **strongest for Android**, with **UiHound**, **ViewScope**, and **uiautodev** offering mature, actively maintained web-based inspectors with locator generation and remote control capabilities [citation:2][citation:3][citation:6]. **ui-finder** is notable for its zero-setup philosophy [citation:5], while **Smart XPath Locator** fills a Windows desktop niche with Excel export [citation:1]. For **iOS**, **Treescope** is the leading open-source option, uniquely providing full SwiftUI inspection in a browser without installing a separate app [citation:8]. For **React Native** developers, **react-native-element-inspector** offers an in-app inspection experience that requires no external tooling [citation:13]. No single open-source tool covers all platforms equally well—the right choice depends on whether your primary target is Android, iOS, or a cross-platform framework.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
