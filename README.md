# r2-workspace-swift
A workspace for on-boarding developers

This workspace is one of the ways you can get started with the R2 Swift Projects. It is not the only way and you can pick to setup your development environment in the way that best fits your needs.

### Prerequisite
- install/update [Carthage](https://github.com/Carthage/Carthage)
- install/update [Carting](https://github.com/artemnovichkov/Carting) 
- Xcode 11.x
- Swift 5.3



In this workspace you will find 4 Github branches:

### int/testapp
You pick this branch if are an integrator and all you need is to quickly get started with the R2 Testapp. 

[https://github.com/readium/r2-workspace-swift/tree/int/testapp](https://github.com/readium/r2-workspace-swift/tree/int/testapp)

### dev/testapp
You pick this branch if are an developer and a R2 contributor. You can get started quickly on the R2 Testapp and it's modules with this branch. We do appreciate any contribution, no matter how small it is, it makes a difference :) 

[https://github.com/readium/r2-workspace-swift/tree/dev/testapp](https://github.com/readium/r2-workspace-swift/tree/dev/testapp)

### int/testapp-with-lcp
You pick this branch if are an integrator and you would like to get started with the R2 Testapp supporting LCP. 

Warning: the content of this branch cannot be built without adding a pre-compiled Readium LCP module. Read below about how you can obtain it.

[https://github.com/readium/r2-workspace-swift/tree/int/testapp-with-lcp](https://github.com/readium/r2-workspace-swift/tree/int/testapp-with-lcp)

### dev/testapp-with-lcp
You pick this branch if are an developer and a R2 contributor. You can get started quickly on the R2 Testapp and it's modules including LCP with this branch. We do appreciate any contribution, no matter how small it is, it makes a difference :) 

Warning: the content of this branch cannot be built without adding a pre-compiled Readium LCP module. Read below about how you can obtain it.

[https://github.com/readium/r2-workspace-swift/tree/dev/testapp-with-lcp](https://github.com/readium/r2-workspace-swift/tree/dev/testapp-with-lcp)


## Getting the pre-compiled Readium LCP module.

Readium LCP is a DRM: as any protection technology, care must be taken to avoid disclosing too much technical information to the open world without good reasons. And Readium LCP, in its "production" profile, is subject to annual licensing fees. 

EDRLab has chosen to provide a small pre-compiled Readium LCP module to R2 implementers, in two flavors: "test" grade and "production" grade. The  -with-lcp branches above cannot be built without the "test" or "prodution" grade LCP library. If you try you'll get an error: No such module 'R2LCPClient'.

1. the "test" grade LCP library is provided after a direct contact between the developer and EDRLab. To get this library, a developer must only provide to EDRLab via a simple form its company name, web site and basic information about the context of the project involving Readium LCP.
2.  the "production" grade LCP library will simply replace the "test" library in the project after the development has been fully tested. Go get access to this production module, a contract must have been signed between the client company and EDRLab and annual licensing fees must have been agreed on.

To contact EDRLab, please send an email to contact(at)edrlab.org or use the Readium Slack on the "lcp" channel.

