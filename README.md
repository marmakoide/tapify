# tapify

This utility is specific to the Oric 1 and Oric Atmos microcomputers. It takes 
a raw binary file and outputs a tape file to run that binary either on a real
computer or an emulated one.

## Getting started 

### Prerequisites

You will need

* Python 2.7 or above)


### Usage

A typical use case is to turn a binary *game.bin* into the *game.tap* file:

```
tapify --autorun game.bin game.tap
```

The *--autorun* switch specifies that the binary should be launched as soon
as it is completly loaded into the Oric's memory, using the command *CLOAD"*

By default, the start address for the binary is set to 0x500, aka the lowest
address available for user programs on Oric computers. You can modify this
with *-s* or *--start-address* switch.

In any cases, you can get informations about the command-line parameters with
the --help switch

```
tapify --help
```

## Authors

* **Alexandre Devert** - *Initial work* - [marmakoide](https://github.com/marmakoide)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details


