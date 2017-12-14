# EdenUnit GUI client

# BEFORE USING EDENUNIT SIMPLEWALLET/DAEMON OR EUROBIT GUI CLIENT:
## If your daemon is stuck on block 0, or if you do not have any peers, load up the daemon and start it like the following:
> ./edenunitd --add-peer put.seed.node.here:8080

Or

> ./edenunitd --add-peer put.seed.node.here:8080
## Doing this will manually connect you to the seed nodes to allow you to find more peers, if the daemon or GUI client is starting at block 0 exit both and open the daemon with that command, then you may continue to use simplewallet once it is done syncing, or once it is done syncing close the daemon and open up the GUI client and it should start getting blocks as it should normally
# How to compile EdenUnit GUI wallet

This is assuming you are running on Ubuntu, replace the download commands with the corresponding commands to your OS
If you are on Windows just download the binarys, no compile needed :D (or download linux binarys)

## Clone the GUI wallet source/Edenunit Source

> git clone https://github.com/EdenUnitDev/Edenunit_GUI_Client

> git clone https://github.com/EdenUnitDev/EdenUnit

Put Edenunit in the Edenunit_GUI_Client edenunit-gui folder and rename edenunit-master to "cryptonote"


## Download Dependencies

> sudo apt-get install build-essential git cmake libboost1.55-all-dev
> sudo apt-get install qt5-default

## Make a build folder

Make a folder to hold the build by doing the command

>mkdir build

## CD to your build folder

> cd build

## cmake the make files

While in your build folder, do this command to create the make files

> cmake [the file path cmakelists.txt in Edenunit GUI folder]

To find the filepath of the edenunit_gui, simply drag the edenunit_gui folder into the terminal, it should show a filepath,
then copy and paste that filepath infront of cmake

## make the GUI wallet

After cmake is done building the make file, simply do the command

> make

If your on a system with a multi core CPU you can do this command to speed up the compile:

> make -j (Number of threads)

Note: The compile may take a while

## Your wallet is compiled

Once make is done compiling the source, simply go to the build folder and run the GUI wallet and begin to sync with the blockchain
