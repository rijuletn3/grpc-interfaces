> :warning: The Cartesi team keeps working internally on the next version of this repository, following its regular development roadmap. Whenever there's a new version ready or important fix, these are published to the public source tree as new releases.

# Cartesi gRPC Interfaces

The Cartesi gRPC Interfaces repository contains all gRPC and Protobuf definitions used in the gRPC interfaces of the Cartesi Project modules. Currently these comprehend:

- [cartesi-base.proto](cartesi-base.proto): basic message types used in multiple interfaces
- [core.proto](core.proto): services exported by the machine emulator and used by the machine manager
- [manager-low.proto](manager-low.proto): services and higher level message types used by the machine emulator to interact with the machine manager
- [manager-high.proto](manager-high.proto): services and higher level message types used to interact with the machine manager sessions
- [logger-high.proto](logger-high.proto): services and higher level message types used to interact with the logger manager sessions

## Getting Started

This repository is not intended for standalone usage. Every repository that makes use of a gRPC interface, either serving or consuming a certain API, includes this repository as submodule and builds the language specific auto-generated code that implements the desired services and messages. Specifics on those can be checked in the individual repositories that include this as a submodule.

## Contributing

Thank you for your interest in Cartesi! Head over to our [Contributing Guidelines](CONTRIBUTING.md) for instructions on how to sign our Contributors Agreement and get started with Cartesi!

Please note we have a [Code of Conduct](CODE_OF_CONDUCT.md), please follow it in all your interactions with the project.

## Authors

* *Diego Nehab*
* *Carlo Fragni*
* *Augusto Teixeira*

## License

The grpc-interfaces repository and all contributions are licensed under [APACHE 2.0](https://www.apache.org/licenses/LICENSE-2.0). Please review our [LICENSE](LICENSE) file.

## Acknowledgments

- Original work 
