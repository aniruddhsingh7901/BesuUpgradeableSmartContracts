
1.A CreateX contract factory is just a smart contract designed to deploy other smart contracts in a standardized way, using the Create2 method. This ensures that the deployed contracts will always be at the same address, regardless of which network they are on. It makes it easier to manage and interact with smart contracts across different blockchain networks.
2.All the contracts are deployed using CreateX contract factories via deployCreate2(salt,initCode) function, so reside on the same addresses across all networks deployed.
3.The contracts were deployed via TransparentUpgradeableProxy pattern, so they can be upgraded by our team in the future if needed.






























# BesuUpgradeableSmartContracts
This repository contains smart contracts deployed on a Besu private network using the Create2 factory pattern. The contracts follow the TransparentUpgradeableProxy pattern, enabling future upgrades by the development team. All deployed contracts share unified addresses across networks, allowing for seamless interaction and updates. 
