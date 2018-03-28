# Timing DAQ repository

The main aim of this code is to convert raw binary data recorded from SiPMs from different devices and analyze them in a coherent and standardised way.
The main executable applications will be created by the istallation in the main folder. One for each available device is present under the form: ``<device_name>Dat2Root``.

## Quick start
If you are not interested in the details just use the following commands

### Installation
To install copy paste the following::
git clone https://github.com/CaltechPrecisionTiming/TimingDAQ
make -j8


### Examples

``./DRSDat2Root --input_file=<your_file>.dat --config=config/DRS_Na22.config --N_evts=10000``

## Command line options
All the command line option must be passed using the sintax ``--<opt>=<val>``.
The following option are common to all the devices.

Compulsory arguments don't have default value

| Argument | Default | Notes|
| -------- | :-------: | ---- |
|``input_file``|    |Binary input file with the data. Must end in ``.dat``.|
|``config``       |Configuration file (see below).|
``output_file``| ``<input>.root`` | Output root file containing a singe tree called ``pulse``. If not provided, the default option is to have the same name of the input file with the ``.root`` extension.|

### VME additional options:

example

### DRS additional options:

TODO: instructions

## Configuration file
