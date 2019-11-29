# r2-workspace-swift
A workspace for on-boarding developers

This workspace is one of the ways you can get started with the R2 Swift Projects. It is not the only way and you can pick to setup your developement environment in the way that best fits your needs.

This is one of the 4 Github branches in this workspace:

### int/testapp-with-lcp
You pick this branch if are an integrator and you would like to get started with the R2 Testapp supporting LCP. 

### Prerequisite
- install/update [Carthage](https://github.com/Carthage/Carthage)
- install/update [Carting](https://github.com/artemnovichkov/Carting) 
- Xcode 10.x
- Swift 4.2

### Setup your workspace

1. git clone --recurse-submodules -b int/testapp-with-lcp  https://github.com/readium/r2-workspace-swift.git r2-workspace-swift
2. add your lcp dependency to the cartfile
3. run **carthage update --platform ios** on r2-testapp-swift
4. run **carting update** on r2-testapp-swift
5. open **r2-workspace-swift.xcworkspace**
6. run target **r2-testapp-swift (carthage-with-lcp)**

**Cartfile should look like this:**

```
github "readium/r2-shared-swift" == ?.?.?
github "readium/r2-streamer-swift" == ?.?.?
github "readium/r2-navigator-swift" == ?.?.?
github "readium/readium-opds-swift" == ?.?.?
github "weichsel/ZIPFoundation" == 0.9.8
github "onevcat/Kingfisher" == 4.10.1
github "jdg/MBProgressHUD"
github "stephencelis/SQLite.swift" == 0.11.5
github "tadija/AEXML" == 4.3.3
github "swisspol/GCDWebServer" == 3.5.2
github "krzyzanowskim/CryptoSwift" == 0.15.0
github "cezheng/Fuzi" == 2.2.1
github "dexman/Minizip"
```
- [weichsel/ZIPFoundation](https://github.com/weichsel/ZIPFoundation) used in [ReadiumLCP](https://github.com/readium/r2-lcp-swift)
- [onevcat/Kingfisher](https://github.com/onevcat/Kingfisher) used in [R2 Testapp](https://github.com/readium/r2-testapp-swift)
- [jdg/MBProgressHUD](https://github.com/jdg/MBProgressHUD) used in [R2 Testapp](https://github.com/readium/r2-testapp-swift)
- [stephencelis/SQLite.swift](https://github.com/stephencelis/SQLite.swift) used in [R2 Testapp](https://github.com/readium/r2-testapp-swift), [ReadiumLCP](https://github.com/readium/r2-lcp-swift)
- [tadija/AEXML](https://github.com/tadija/AEXML) used in [R2Streamer](https://github.com/readium/r2-streamer-swift)
- [swisspol/GCDWebServer](https://github.com/swisspol/GCDWebServer) used in [R2Streamer](https://github.com/readium/r2-streamer-swift)
- [krzyzanowskim/CryptoSwift](https://github.com/krzyzanowskim/CryptoSwift) used in [ReadiumLCP](https://github.com/readium/r2-lcp-swift), [R2Streamer](/readium/r2-streamer-swift)
- [cezheng/Fuzi](https://github.com/cezheng/Fuzi) used in [ReadiumOPDS](https://github.com/readium/r2-opds-swift), [R2Streamer](https://github.com/readium/r2-streamer-swift)
- [dexman/Minizip](https://github.com/dexman/Minizip) used in [R2Streamer](https://github.com/readium/r2-streamer-swift)


## Getting the pre-compiled Readium LCP module.

Readium LCP is a DRM. As any protection technology, care must be taken to avoid disclosing too much technical information to the open world without good reasons. This is why EDRLab has chosen to provide a small pre-compiled Readium LCP module to R2 implementers, in two flavors:

1. a "test" grade LCP library, provided after a direct contact between the developer and EDRLab. To get this library, a developer must only provide to EDRLab its company name, web site and basic information about the context of the project involving Readium LCP.
2.  a "production" grade LCP library, which simply replaces the "test" library in the project after the development has been fully tested. Go get access to this production module, the client company must be trusted and the Readium LCP Terms of Used must have been signed.

To contact EDRLab, please send an email to contact(at)edrlab.org or use the Readium Slack on the "lcp" channel.

