# r2-workspace-swift
A workspace for on-boarding developers

This workspace is one of the ways you can get started with the R2 Swift Projects. It is not the only way and you can pick to setup your development environment in the way that best fits your needs.

This is one of the 4 Github branches in this workspace:

### int/testapp
You pick this branch if are an integrator and all you need is to quickly get started with the R2 Testapp. 

### Prerequisite
- install/update [Carthage](https://github.com/Carthage/Carthage)
- install/update [Carting](https://github.com/artemnovichkov/Carting) 
- Xcode 10.x
- Swift 4.2

### Setup your workspace

1. git clone --recurse-submodules -b int/testapp https://github.com/readium/r2-workspace-swift.git
2. ckeckout **int/testapp** branch **including it's submodules**
3. run **carthage update --platform ios** on r2-testapp-swift
8. run **carting update** on r2-testapp-swift
4. open **r2-workspace-swift.xcworkspace**
5. run target **r2-testapp-swift (carthage)**

**Cartfile should look like this:**

```
github "readium/r2-shared-swift" "develop"
github "readium/r2-streamer-swift" "develop"
github "readium/r2-navigator-swift" "develop"
github "readium/readium-opds-swift" "develop"
github "edrlab/ZIPFoundation" "master"
github "onevcat/Kingfisher" == 4.6.4
github "jdg/MBProgressHUD" ~> 1.1.0
github "stephencelis/SQLite.swift" == 0.11.5
github "tadija/AEXML" == 4.3.3
github "swisspol/GCDWebServer" == 3.5.2
github "krzyzanowskim/CryptoSwift" == 0.14.0
github "cezheng/Fuzi" == 2.1.0
github "dexman/Minizip"
```
- [edrlab/ZIPFoundation](edrlab/ZIPFoundation) used in [ReadiumLCP](readium/r2-lcp-swift)
- [onevcat/Kingfisher](onevcat/Kingfisher) used in [R2 Testapp](readium/r2-testapp-swift)
- [jdg/MBProgressHUD](jdg/MBProgressHUD) used in [R2 Testapp](readium/r2-testapp-swift)
- [stephencelis/SQLite.swift](stephencelis/SQLite.swift) used in [R2 Testapp](readium/r2-testapp-swift), [ReadiumLCP](readium/r2-lcp-swift)
- [tadija/AEXML](tadija/AEXML) used in [R2Streamer](readium/r2-streamer-swift)
- [swisspol/GCDWebServer](swisspol/GCDWebServer) used in [R2Streamer](readium/r2-streamer-swift)
- [krzyzanowskim/CryptoSwift](krzyzanowskim/CryptoSwift) used in [ReadiumLCP](readium/r2-lcp-swift), [R2Streamer](readium/r2-streamer-swift)
- [cezheng/Fuzi](cezheng/Fuzi) used in [ReadiumOPDS](readium/r2-opds-swift), [R2Streamer](readium/r2-streamer-swift)
- [dexman/Minizip](dexman/Minizip) used in [R2Streamer](readium/r2-streamer-swift)

