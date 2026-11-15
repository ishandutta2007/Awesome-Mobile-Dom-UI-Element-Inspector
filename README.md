# Awesome Mobile DOM & UI Element Inspector

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/ishandutta2007/Awesome-Mobile-Dom-UI-Element-Inspector/pulls)
[![GitHub stars](https://img.shields.io/github/stars/ishandutta2007/Awesome-Mobile-Dom-UI-Element-Inspector?style=social)](https://github.com/ishandutta2007/Awesome-Mobile-Dom-UI-Element-Inspector/stargazers)

> A curated list of top **Mobile DOM & UI Element Inspector** platforms, view hierarchy debuggers, XPath/locator generators, and layout inspection developer tools — covering commercial cloud device farms, SaaS testing suites, and open-source software for Android, iOS, React Native, and HarmonyOS.
>
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [Sector Overview & Market Dynamics](#-sector-overview--market-dynamics)
- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
- [Open-Source Software](#-open-source-software)
  - [Flipper](#flipper)
  - [Appium Inspector](#appium-inspector)
  - [Lookin](#lookin)
  - [WEditor](#weditor)
  - [ViewMonitor](#viewmonitor)
  - [uiautodev](#uiautodev)
  - [Macaca App Inspector](#macaca-app-inspector)
  - [UInspector](#uinspector)
  - [UI Viewer](#ui-viewer)
  - [Cutaway](#cutaway)
  - [Android Inspector](#android-inspector)
  - [Treescope](#treescope)
  - [React Native Element Inspector](#react-native-element-inspector)
  - [ViewScope](#viewscope)
  - [UiHound](#uihound)
  - [ui-finder](#ui-finder)
- [Feature Comparison Matrix](#-feature-comparison-matrix)
- [Contributing](#-contributing)
- [License](#-license)

---

## 📈 Sector Overview & Market Dynamics

The global **Mobile Application Testing and Quality Engineering Market** is valued between **$8.6 Billion and $11.7 Billion** (projected to exceed $33 Billion by 2035 at an estimated CAGR of 13%–16%). 

The sector is **moderately fragmented**: while massive capital expenditure requirements for physical real-device clouds concentrate hosted infrastructure and device farms among a few multi-billion-dollar leaders (such as BrowserStack and Sauce Labs), the tooling and inspector ecosystem remains dynamic and competitive, with nimble innovators (LambdaTest, Kobiton) and open-source automation standards (Appium, Flipper, WEditor) continuously evolving to address emerging mobile frameworks, OS updates, and AI-driven locator generation.

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Mobile DOM, view hierarchy, and element inspector platforms. The table below is sorted in descending order by company scale (valuation and annual revenue).

| Platform | Starting Tier Pricing | Free Tier / Trial Limit | Company Scale (Valuation / Revenue) | Target OS & Coverage | Key Strengths |
|----------|-----------------------|-------------------------|------------------------------------|----------------------|---------------|
| **[BrowserStack](https://www.browserstack.com/)** | **$29/month** (Live Web, billed annually) / **$39/month** (App Live) | **Free Trial:** 30 minutes manual Live/App Live testing, 100 screenshots, 60–100 automated test minutes | **$4.0B Valuation** (~$200M+ est. ARR) | Android, iOS, Mobile Web, Desktop | Real-device cloud with live interactive DOM inspector, device rotation, geolocation, and Percy visual testing. |
| **[Sauce Labs](https://saucelabs.com/)** | **$199/month** (Live & Real Device Testing, billed annually) | **28-Day Free Trial:** 60 automated & live test minutes, virtual/real mobile devices, local Sauce Connect tunnel | **$613M Valuation** (~$70M–$90M est. ARR) | Android, iOS, Simulators, Emulators | Live DOM element inspector, deep Appium integration, enterprise device clouds, test orchestration, and error analytics. |
| **[LambdaTest](https://www.lambdatest.com/)** | **$15/month** (Live Testing) / **$79/month** (Mobile App & Web Automation) | **Free Forever Plan:** 60 minutes/month live browser testing (10-min sessions), 10 responsive tests, 1 parallel session | **$400M Valuation** (~$20M–$25M est. ARR) | Android, iOS, Mobile Browsers, Real Devices | Web-based real-time mobile DOM inspector, interactive debugging, KaneAI automation, and low-latency virtual cloud. |
| **[Kobiton](https://kobiton.com/)** | **$83/month** (Startup Plan with ~500 real-device minutes/month) | **14-Day Free Trial:** 300 minutes on real mobile devices, sample AI script generation, no credit card required | **$65M Valuation** (~$27M est. ARR) | Android, iOS, Tablets, Wearables | Embedded Session Explorer inspector with live XPath capture, visual validations, and bidirectional Appium Inspector integration. |

---

## 🟩 Open-Source Software

Self-hosted, community-driven Mobile DOM and UI element inspector tools. Sorted in descending order by GitHub star count.

### Flipper
[![GitHub stars](https://img.shields.io/github/stars/meta/flipper?style=social&color=white)](https://github.com/meta/flipper/stargazers)
- **Repository:** [meta/flipper](https://github.com/meta/flipper)
- **Stack:** TypeScript / C++ / Electron | **License:** MIT
- **Platform:** iOS, Android, React Native
- **Overview:** Flipper is Meta's extensible desktop debugging platform for mobile app development. Its Layout Inspector lets developers explore the complete native view hierarchy (UIKit, Android View/Compose, React Native components), inspect layout properties in real time, visualize boundaries, and modify layout attributes on the fly.

### Appium Inspector
[![GitHub stars](https://img.shields.io/github/stars/appium/appium-inspector?style=social&color=white)](https://github.com/appium/appium-inspector/stargazers)
- **Repository:** [appium/appium-inspector](https://github.com/appium/appium-inspector)
- **Stack:** Electron / React / TypeScript | **License:** Apache-2.0
- **Platform:** Android, iOS, Windows, macOS
- **Overview:** The official GUI inspector for Appium sessions. Displays the interactive view hierarchy, element screenshot overlays, detailed accessibility attributes, and automatic locator suggestions (ID, accessibility ID, XPath, UIAutomator, iOS Class Chain). Standalone desktop app available across macOS, Windows, and Linux.

### Lookin
[![GitHub stars](https://img.shields.io/github/stars/hughkli/Lookin?style=social&color=white)](https://github.com/hughkli/Lookin/stargazers)
- **Repository:** [hughkli/Lookin](https://github.com/hughkli/Lookin)
- **Stack:** Objective-C / Swift / macOS App | **License:** GPL-3.0
- **Platform:** iOS
- **Overview:** A premier free macOS app for iOS view debugging and inspection, serving as a powerful open alternative to Reveal and Xcode View Debugger. Features 2D/3D hierarchy inspection, live property editing, layer wireframing, and performance metrics for UIKit applications.

### WEditor
[![GitHub stars](https://img.shields.io/github/stars/alibaba/web-editor?style=social&color=white)](https://github.com/alibaba/web-editor/stargazers)
- **Repository:** [alibaba/web-editor](https://github.com/alibaba/web-editor)
- **Stack:** Python / Tornado / Web UI | **License:** Apache-2.0
- **Platform:** Android, iOS
- **Overview:** Web-based UI inspector and script editor created for `uiautomator2` and `facebook-wda`. Captures real-time device screen dumps, renders interactive node trees, and allows engineers to test and generate robust XPath and UI selectors directly inside any web browser.

### ViewMonitor
[![GitHub stars](https://img.shields.io/github/stars/daisuke0131/ViewMonitor?style=social&color=white)](https://github.com/daisuke0131/ViewMonitor/stargazers)
- **Repository:** [daisuke0131/ViewMonitor](https://github.com/daisuke0131/ViewMonitor)
- **Stack:** Swift | **License:** MIT
- **Platform:** iOS
- **Overview:** An in-app visual layout inspector for iOS that operates directly on device. It inspects UIKit and SwiftUI views, frames, layout margins, padding, spacing, view overlaps, and intrinsic content sizes without requiring tethered desktop software.

### uiautodev
[![GitHub stars](https://img.shields.io/github/stars/codeskyblue/uiautodev?style=social&color=white)](https://github.com/codeskyblue/uiautodev/stargazers)
- **Repository:** [codeskyblue/uiautodev](https://github.com/codeskyblue/uiautodev)
- **Stack:** Python / Prebuilt Binary / Web UI | **License:** MIT
- **Platform:** Android, iOS, HarmonyOS
- **Overview:** Next-generation browser-based mobile UI viewer and inspector supporting Android, iOS, and HarmonyOS. Features tree-based element inspection, automatic XPath locator generation, offline snapshot analysis, and standalone client binaries with zero setup.

### Macaca App Inspector
[![GitHub stars](https://img.shields.io/github/stars/macacajs/app-inspector?style=social&color=white)](https://github.com/macacajs/app-inspector/stargazers)
- **Repository:** [macacajs/app-inspector](https://github.com/macacajs/app-inspector)
- **Stack:** Node.js / JavaScript | **License:** MIT
- **Platform:** Android, iOS
- **Overview:** Macaca's web-based mobile UI viewer and element inspector. Provides interactive DOM and UI hierarchy viewing in a browser, element attribute inspection, and locator code generation for cross-platform automation suites.

### UInspector
[![GitHub stars](https://img.shields.io/github/stars/YvesCheung/UInspector?style=social&color=white)](https://github.com/YvesCheung/UInspector/stargazers)
- **Repository:** [YvesCheung/UInspector](https://github.com/YvesCheung/UInspector)
- **Stack:** Kotlin / Java | **License:** Apache-2.0
- **Platform:** Android
- **Overview:** An on-device UI inspection library for Android that traverses view hierarchies at runtime. Tap any screen element to reveal parent/child relationships, examine LayoutParams, inspect view backgrounds, fonts, and view lifecycle states right on the device screen.

### UI Viewer
[![GitHub stars](https://img.shields.io/github/stars/codematrixer/ui-viewer?style=social&color=white)](https://github.com/codematrixer/ui-viewer/stargazers)
- **Repository:** [codematrixer/ui-viewer](https://github.com/codematrixer/ui-viewer)
- **Stack:** Python / Web UI | **License:** MIT
- **Platform:** Android, iOS, HarmonyOS NEXT
- **Overview:** A lightweight UI hierarchy inspector for mobile applications with native support for Android, iOS, and HarmonyOS NEXT. Visualizes screen dumps alongside control trees, extracts selector properties, and calculates unique locators.

### Cutaway
[![GitHub stars](https://img.shields.io/github/stars/nothingsh/Cutaway?style=social&color=white)](https://github.com/nothingsh/Cutaway/stargazers)
- **Repository:** [nothingsh/Cutaway](https://github.com/nothingsh/Cutaway)
- **Stack:** Swift / macOS Native | **License:** MIT
- **Platform:** iOS
- **Overview:** A standalone macOS application for inspecting the layer hierarchy of iOS apps. Renders visual 3D exploded views of views and layers, helping developers uncover hidden views, clip-to-bounds bugs, and incorrect z-index ordering.

### Android Inspector
[![GitHub stars](https://img.shields.io/github/stars/cmzf/android-inspector?style=social&color=white)](https://github.com/cmzf/android-inspector/stargazers)
- **Repository:** [cmzf/android-inspector](https://github.com/cmzf/android-inspector)
- **Stack:** Java / Web UI | **License:** Apache-2.0
- **Platform:** Android
- **Overview:** A productive UI layout inspector app for Android and Appium with an embedded HTTP server. Serves as a modern, high-speed drop-in replacement for the legacy `uiautomatorviewer` (`monitor.bat`), providing instant layout dumps and XPath queries.

### Treescope
[![GitHub stars](https://img.shields.io/github/stars/everettjf/treescope?style=social&color=white)](https://github.com/everettjf/treescope/stargazers)
- **Repository:** [everettjf/treescope](https://github.com/everettjf/treescope)
- **Stack:** Swift / TypeScript | **License:** MIT
- **Platform:** iOS, macOS
- **Overview:** An open-source runtime view inspector for UIKit, AppKit, and SwiftUI viewed entirely inside a web browser. Serves as a zero-install alternative to Lookin with first-class SwiftUI support, unwrapping complex views, `@State`, and modifier pipelines.

### React Native Element Inspector
[![GitHub stars](https://img.shields.io/github/stars/mabdinasira/react-native-element-inspector?style=social&color=white)](https://github.com/mabdinasira/react-native-element-inspector/stargazers)
- **Repository:** [mabdinasira/react-native-element-inspector](https://github.com/mabdinasira/react-native-element-inspector)
- **Stack:** React Native / TypeScript | **License:** MIT
- **Platform:** iOS, Android (React Native)
- **Overview:** An on-device "Inspect Element" developer utility for React Native apps. Tap any UI component to view CSS styles, toggle properties in real time, examine box-model margins/padding overlays, and jump to source code definitions without external native dependencies.

### ViewScope
[![GitHub stars](https://img.shields.io/github/stars/wangwanjie/ViewScope?style=social&color=white)](https://github.com/wangwanjie/ViewScope/stargazers)
- **Repository:** [wangwanjie/ViewScope](https://github.com/wangwanjie/ViewScope)
- **Stack:** Swift / AppKit | **License:** MIT
- **Platform:** macOS, iOS
- **Overview:** A macOS desktop utility for inspecting and visualizing UI view hierarchies, designed to help developers debug and analyze app layouts in real time with 2D/3D hierarchy wireframing and attribute panes.

### UiHound
[![GitHub stars](https://img.shields.io/github/stars/duzitian-code/UIHound?style=social&color=white)](https://github.com/duzitian-code/UIHound/stargazers)
- **Repository:** [duzitian-code/UIHound](https://github.com/duzitian-code/UIHound)
- **Stack:** Python / FastAPI / Web UI | **License:** Open Source
- **Platform:** Android
- **Overview:** A local browser-based Android UI debugging and automation workbench for HIL testing. Features interactive hierarchy inspection, unique locator generation, remote device control via scrcpy, pixel color sampling, and offline snapshot viewing.

### ui-finder
[![GitHub stars](https://img.shields.io/github/stars/kdiitg/ui_finder?style=social&color=white)](https://github.com/kdiitg/ui_finder/stargazers)
- **Repository:** [kdiitg/ui_finder](https://github.com/kdiitg/ui_finder)
- **Stack:** Python | **License:** Open Source
- **Platform:** Android
- **Overview:** A plug-and-play Python visual tool for inspecting Android application UIs directly from a connected device. Provides zero-setup dependency installation, click-to-highlight element selection, dropdown filtering by class/ID, and instant locator copying.

---

## 📊 Feature Comparison Matrix

| Tool | Type | License | Primary Platforms | Locator Generation | Live Device / Remote Control | Runtime Inspection Mode |
|------|------|---------|-------------------|--------------------|-----------------------------|-------------------------|
| **[BrowserStack](https://www.browserstack.com/)** | SaaS | Commercial | Android, iOS, Web | ✅ Interactive | ✅ Real-device cloud | Cloud Streaming & DOM DevTools |
| **[Sauce Labs](https://saucelabs.com/)** | SaaS | Commercial | Android, iOS, Web | ✅ XPath / ID | ✅ Real-device & Virtual | Cloud Session Debugger |
| **[LambdaTest](https://www.lambdatest.com/)** | SaaS | Commercial | Android, iOS, Web | ✅ Selector Engine | ✅ Real-device & Virtual | Cloud Live DevTools |
| **[Kobiton](https://kobiton.com/)** | SaaS | Commercial | Android, iOS | ✅ XPath / Appium | ✅ Cloud & Local Devices | Session Explorer Inspector |
| **[Flipper](https://github.com/meta/flipper)** | Open Source | MIT | iOS, Android, RN | ❌ | ✅ USB / WiFi | Desktop Client + In-App SDK |
| **[Appium Inspector](https://github.com/appium/appium-inspector)** | Open Source | Apache-2.0 | Android, iOS | ✅ Multi-strategy | ✅ Via Appium Server | Desktop GUI Inspector |
| **[Lookin](https://github.com/hughkli/Lookin)** | Open Source | GPL-3.0 | iOS | ❌ | ✅ USB / WiFi | macOS Client + In-App Server |
| **[WEditor](https://github.com/alibaba/web-editor)** | Open Source | Apache-2.0 | Android, iOS | ✅ uiautomator / XPath | ✅ ADB / WDA | Web Browser UI |
| **[ViewMonitor](https://github.com/daisuke0131/ViewMonitor)** | Open Source | MIT | iOS | ❌ | ✅ On-device | In-App Overlay View |
| **[uiautodev](https://github.com/codeskyblue/uiautodev)** | Open Source | MIT | Android, iOS, Harmony | ✅ XPath & Scripts | ✅ ADB / idb / hdc | Browser UI + Local Server |
| **[Macaca App Inspector](https://github.com/macacajs/app-inspector)** | Open Source | MIT | Android, iOS | ✅ XPath & Macaca | ✅ USB Connection | Browser UI |
| **[UInspector](https://github.com/YvesCheung/UInspector)** | Open Source | Apache-2.0 | Android | ❌ | ✅ On-device | In-App Floating Panel |
| **[UI Viewer](https://github.com/codematrixer/ui-viewer)** | Open Source | MIT | Android, iOS, Harmony | ✅ XPath | ✅ USB Connection | Web Browser UI |
| **[Cutaway](https://github.com/nothingsh/Cutaway)** | Open Source | MIT | iOS | ❌ | ✅ USB Connection | macOS Desktop 3D Window |
| **[Android Inspector](https://github.com/cmzf/android-inspector)** | Open Source | Apache-2.0 | Android | ✅ XPath | ✅ ADB Live Sync | Embedded Web Server |
| **[Treescope](https://github.com/everettjf/treescope)** | Open Source | MIT | iOS, macOS | ❌ | ✅ Loopback HTTP | Embedded Web Viewer |
| **[React Native Element Inspector](https://github.com/mabdinasira/react-native-element-inspector)** | Open Source | MIT | React Native | ❌ | ✅ In-app | On-Screen Overlay |
| **[ViewScope](https://github.com/wangwanjie/ViewScope)** | Open Source | MIT | macOS, iOS | ❌ | ✅ Local Mac | macOS App Window |
| **[UiHound](https://github.com/duzitian-code/UIHound)** | Open Source | Proprietary | Android | ✅ u2 / XPath | ✅ scrcpy Remote | Web Browser UI |
| **[ui-finder](https://github.com/kdiitg/ui_finder)** | Open Source | Proprietary | Android | ✅ Attributes | ✅ ADB Live Screen | Desktop Matplotlib Window |

---

## 🤝 Contributing

Contributions are warmly welcome! If you know of an actively maintained mobile DOM, view hierarchy, or layout inspector tool that should be included:

1. Fork this repository.
2. Add the tool to the appropriate section in alphabetical or sorted order.
3. Include the repository URL, star badge (`shields.io` social style), platform support, and a concise 1–2 sentence description.
4. Submit a Pull Request with a clear description of why the tool is valuable to mobile engineers.

---

## 📄 License

This collection is published under the [Creative Commons Zero v1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) (CC0 1.0) Public Domain Dedication. Listed tools and third-party projects retain their respective trademarks and open-source licenses.

---

<p align="center">
  <sub>Maintained with ❤️ for the mobile engineering, QA automation, and developer tooling community.</sub>
</p>
