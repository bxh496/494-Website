##### [Home](README.md) &nbsp; | &nbsp; [Education](education.md) &nbsp; | &nbsp; [Past Projects](projects.md) &nbsp; | &nbsp; [Work Experience](experience.md) &nbsp; | &nbsp; [Senior Design](sDesign.md) &nbsp; | &nbsp; [Reflections](reflections.md)

# Past Projects

## 309 Group Design Project
### Project Description

## 327 Sound Generation Project
### Project Description
This project was a part of our advanced programming course. The idea behind the project was to create a multi part program which could perform various actions when working with a custom defined sound file. The different components described below are as follows: sndcat, sndinfo, sndmix, and sndgen. The cs229 files could be converted to a proper .wav format through an executable provided by the instructor. The project was developed in C++ by myself.

#### The sound file
The file format was defined as .cs229. It consisted of a header followed by line separated sample values. The header consisted of bit resolution, the sample rate, number of channels to play on, and optionally the number of the samples in the file.
#### sndinfo
This executable is used to provide information on a file given to it. It parses the file and outputs the filename/extension, the length in seconds the file would play, and the 4 pieces information contained in the header of the sound file.
#### sndcat
This executable takes as arguments valid cs229 files and concatenates them in the order given. It deals with header mismatches between files in various ways. User can specify an output file or the program will send it to cout.
#### sndmix
This executable mixes a number of sound files together by adding the sample values on corresponding line between the files together. Each file could also have a multiplier defined on it to change how strongly it affected the output file.
#### sndgen
This is the most interesting of the executables. It takes user selected flags to generate sound waves in cs229 format using an ADSR envelope in a few different wave shapes.

### Takeaway
This was my first major assignment in C++ and the sheer size of it forced me to learn a lot about the language. We were given a lot of freedom in how to tackle the problems and inheritance hierarchy used, which meant it was pretty much up to me to solve my own problems and deal with any roadblocks in the language I hit.

## 530 Packet Decoder
### Project Description
This project was an effort in properly understanding packet headers and how the data gets parsed by the operating system. The professor provided us with a base program which would capture the packets from the NIC and print them out in 16 bit hex values.
