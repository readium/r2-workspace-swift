# r2-workspace-swift
A workspace for on-boarding developers

This workspace is one of the ways you can get started with the R2 Swift Projects. It is not the only way and you can pick to setup your development environment in the way that best fits your needs.

This is one of the 4 GitHub branches in this workspace:

### `dev/testapp`
You pick this branch if are an developer and a R2 contributor. You can get started quickly on the R2 Testapp and it's modules with this branch. We do appreciate any contribution, no matter how small it is, it makes a difference :) 

### Prerequisite

- install/update [Carthage](https://github.com/Carthage/Carthage) 0.38+
- Xcode 12.x
- Swift 5.3

### Setup your workspace

1. run `git clone --recurse-submodules -b dev/testapp https://github.com/readium/r2-workspace-swift.git r2-workspace-swift`
2. comment all `readium/r2-*` dependencies in `r2-testapp-swift/Cartfile`
3. run `carthage update --use-xcframeworks --platform ios` in `r2-testapp-swift/`
4. open `r2-workspace-swift.xcworkspace`
5. build target **r2-testapp-swift (submodules)**

