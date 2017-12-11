# edenunit_gui

# How to compile EdenUnit GUI wallet
This is assuming you are running on Ubuntu, replace the download commands with the corresponding commands to your OS
If you are on Windows just download the binarys, no compile needed :D

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

Note: The compile may take a while

## Your wallet is compiled

Once make is done compiling the source, simply go to the build folder and run the GUI wallet and begin to sync with the blockchain
