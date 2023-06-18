# 🔮 Huddle01 Orb • [![test](https://github.com/orbland/orb/actions/workflows/ci.yml/badge.svg)](https://github.com/orbland/orb/actions/workflows/ci.yml) ![license](https://img.shields.io/badge/License-MIT-green.svg?label=license)

This is a fork of original [Orb](https://github.com/orbland/orb) supports video calls in 

The contract combines the following areas of functionality:

- **Orb and time-gated Video calls.** Allows the Keeper to have a video call via Huddle01 token-gated room with the Orb creator once a week in a predefined time slot.
- **Auction.** Allows the contract owner to start the Orb auction, determining the first Keeper of the Orb.
- **Funds management.** Allows any user to deposit and withdraw funds. Funds are used to make auction bids and pay Harberger Tax.
- **Harberger Tax.** Uses delayed accounting (settling) to allocate funds from the current Keeper to the contract beneficiary, based on the price set by the Keeper and tax rate.
- **ERC-721 compatibility.** All transfers revert, but otherwise, the contract appears as supporting all ERC-721 functions.

## Usage

```shell
forge install foundry-rs/forge-std openzeppelin/openzeppelin-contracts # dependencies
forge test # tests
make anvil # local node
make deploy-anvil # deploy to local node in another terminal
```

## License

Released under the [MIT License](https://github.com/orbland/orb/blob/main/LICENSE).

## Credits

- [Eric Wall](https://twitter.com/ercwl) - Concept and mechanics design
- [Jonas Lekevicius](https://twitter.com/lekevicius) - Contract implementation
- [Odysseas.eth](https://twitter.com/odysseas_eth) - Tests, toolkit setup and many other contributions
- [OpenZeppelin Contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) - Contract is based on OZ ERC-721 and Ownable implementations
