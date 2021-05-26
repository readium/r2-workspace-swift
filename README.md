# r2-workspace-swift
A workspace for on-boarding developers

This workspace is one of the ways you can get started with the R2 Swift Projects. It is not the only way and you can pick to setup your development environment in the way that best fits your needs.

This is one of the 4 Github branches in this workspace:

### `int/testapp`
You pick this branch if are an integrator and all you need is to quickly get started with the R2 Testapp. 

### Prerequisite
- install/update [Carthage](https://github.com/Carthage/Carthage) 0.38+
- Xcode 12.x
- Swift 5.3

### Setup your workspace

1. run `git clone --recurse-submodules -b int/testapp https://github.com/readium/r2-workspace-swift.git r2-workspace-swift`
2. run `carthage update --use-xcframeworks --platform ios` in `r2-testapp-swift/`
3. open `r2-workspace-swift.xcworkspace`
4. build target **r2-testapp-swift (carthage)**

