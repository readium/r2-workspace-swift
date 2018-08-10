# r2-workspace-swift
A workspace for on-boarding developers

This workspace is one of the ways you can get started with the R2 Swift Projects. It is not the only way and you can pick to setup your developement environment in the way that best fits your needs.

This is one of the 4 Github branches in this workspace:

### int/testapp-with-lcp
You pick this branch if are an integrator and you would like to get started with the R2 Testapp supporting LCP. 

1. clone https://github.com/readium/r2-workspace-swift.git
2. ckeckout **int/testapp-with-lcp** branch **including it's submodules**
3. run **carthage update --platform ios** on r2-lcp-swift
3. run **carthage update --platform ios** on r2-testapp-swift
4. copy **liblcp.a** to the root of **r2-lcp-wrapper-swift** directory
5. open **r2-workspace-swift.xcworkspace**
6. run target **r2-testapp-swift (carthage-with-lcp)**


## Getting the pre-compiled Readium LCP module.

Readium LCP is a DRM. As any protection technology, care must be taken to avoid disclosing too much technical information to the open world without good reasons. This is why EDRLab has chosen to provide a small pre-compiled Readium LCP module to R2 implementers, in two flavors:

1. a "test" grade LCP library, provided after a direct contact between the developer and EDRLab. To get this library, a developer must only provide to EDRLab its company name, web site and basic information about the context of the project involving Readium LCP.
2.  a "production" grade LCP library, which simply replaces the "test" library in the project after the development has been fully tested. Go get access to this production module, the client company must be trusted and the Readium LCP Terms of Used must have been signed.

To contact EDRLab, please send an email to contact(at)edrlab.org or use the Readium Slack on the "lcp" channel.

