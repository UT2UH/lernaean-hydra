# Synthetic Data Generator

This the synthetic data generator used in the Lernaean Hydra paper 
on data series similarity search.

The generator produces synthetic data series as random-walks
(i.e., cumulative sums) of steps that follow a Gaussian distribution
(0,1).

## Compile
make

## Run
./generator --help

## Example
export GSL_RNG_SEED=1184
./generator  --size 100000000 --length 256  --z-normalize --filename "data_250M_seed1184_len256_znorm.bin"
