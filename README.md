# networks (private directory)

This repository may contain in the future the networks as required by the NNUE evaluation in Stockfish.
At the time of this writing (12th of August, 2020) this directory has been made private to hide it
and avoid confusion for the general users, because we moved away from github to store networks to a 
dedicated server donated by noobpwnftw (see https://tests.stockfishchess.org/nns). We keep this directory
"just in case" we might want to come back to github to store networks in the future.

## general

The networks follow the naming convention
```
nn-SHA.nnue
```
where SHA are the first 12 digits of the sha256sum of the nn.nnue data file (`sha256sum nn.nnue | cut -c1-12`).

For a given Stockfish version, the default network name (UCI option `EvalFile`),
specifies the compatible and tested network file name. Other combinations may or may not work.

## contributors

Networks that have been successfully tested on fishtest can be added to this repository by pull request.
Such a pull request will be part of a twin PR to the official-stockfish/Stockfish repository that
changes the default value of EvalFile to match the network name.

As a form of documentation, for the benefit of other developers,
the commit message of the pull request should specify basic information
on how the net has been created. Please update the AUTHORS file.
