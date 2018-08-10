# r2-workspace-swift
A workspace for on-boarding developers

This workspace is one of the ways you can get started with the R2 Swift Projects. It is not the only way and you can pick to setup your developement environment in the way that best fits your needs.

This is one of the 4 Github branches in this workspace:


### dev/testapp
You pick this branch if are an developer and a R2 contributor. You can get started quickly on the R2 Testapp and it's modules with this branch. We do appreciate any contribution, no matter how small it is, it makes a difference :) 

1. git clone -b dev/testapp https://github.com/readium/r2-workspace-swift.git
2. ckeckout **dev/testapp** branch **including it's submodules**
3. run **carthage update --platform ios** on r2-shared-swift
4. run **carthage update --platform ios** on r2-streamer-swift
5. run **carthage update --platform ios** on r2-navigator-swift
6. run **carthage update --platform ios** on readium-opds-swift
7. run **carthage update --platform ios** on r2-testapp-swift
8. open **r2-workspace-swift.xcworkspace**
9. run target **r2-testapp-swift (submodules)**

