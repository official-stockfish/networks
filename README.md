# networks

This repository contains the networks as required by the NNUE evaluation in Stockfish.

## general

The networks follow the naming convention
```
nn-SHA.bin
```
where SHA are the first 12 digits of the sha256sum of the nn.bin data file.

For a given Stockfish version, the default network name (UCI option `EvalFile`),
specifies the compatible and tested network file name. Other combinations may or may not work.

## contributors

Networks that have been successfully tested on fishtest can be added to this repository by pull request.
Such a pull request will be part of a twin PR to the official-stockfish/Stockfish repository that
changes the default value of EvalFile to match the network name.

As a form of documentation, for the benefit of other developers,
the commit message of the pull request should specify basic information
on how the net has been created.
