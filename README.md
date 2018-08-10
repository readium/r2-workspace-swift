# r2-workspace-swift
A workspace for on-boarding developers

This workspace is one of the ways you can get started with the R2 Swift Projects. It is not the only way and you can pick to setup your developement environment in the way that best fits your needs.

This is one of the 4 Github branches in this workspace:

### int/testapp
You pick this branch if are an integrator and all you need is to quickly get started with the R2 Testapp. 

1. git clone -b int/testapp https://github.com/readium/r2-workspace-swift.git
2. ckeckout **int/testapp** branch **including it's submodules**
3. run **carthage update --platform ios** on r2-testapp-swift
4. open **r2-workspace-swift.xcworkspace**
5. run target **r2-testapp-swift (carthage)**
