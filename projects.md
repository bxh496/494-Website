##### [Home](README.md) &nbsp; | &nbsp; [Education](education.md) &nbsp; | &nbsp; [Past Projects](projects.md) &nbsp; | &nbsp; [Work Experience](experience.md) &nbsp; | &nbsp; [Senior Design](sDesign.md) &nbsp; | &nbsp; [Reflections](reflections.md)

# Past Projects
#### [Group Design](#gdsgn) &nbsp; | [Sound Project](#snd) &nbsp; | [Packet Decoder](#pkt)

<a name="gdsgn"></a>
## 309 Group Design Project 
### Project Description
This was the first real group project I worked on at Iowa State. The team consisted of 4 of us and took the entirety of the semester to complete. The project itself was a simplistic 2d platforming game we built purely from Java and a simple Swing based graphics/game library we found online to allow for partial map views and whatnot. The players would all move/jump toward the right of the scrolling screen as the map fell away underneath them, multiplayer was achieved via a 'server' host communicating with all players. 

### My role
My contributions to the project most dealt with the back-end logic of how to store the maps, the physics interactions, the map falling away, etc. I also contributed to all of the paperwork we were required to provide for the project.

### Takeaway
This was probably the best class I've taken so far from a documentation standpoint at Iowa State. We were required to go through very detailed design documents and come up with use cases, block diagrams, UML diagrams, the whole nine yards. Future classes which have attempted to achieve similar goals have all fallen short. This class was also my introduction to git, source control obviously being very important when designing anything as a group.

<a name="snd"></a>
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
This was my first major assignment in C++ and the sheer size of it forced me to learn a lot about the language. We were given a lot of freedom in how to tackle the problems and inheritance hierarchy used, which meant it was pretty much up to me to solve my own problems and deal with any roadblocks in the language I hit. The size of the project also forced me to carefully consider and plan my hierarchy and design before I started coding so that I didn't end up having to backtrack hours of work when I realized something wasn't going to work.

<a name="pkt"></a>
## 530 Packet Decoder 
### Project Description
This project was an effort in properly understanding packet headers and how the data gets parsed by the operating system. The professor provided us with a base program which would capture the packets from the NIC and print them out in hexadecimal. Over the course of the semester, I added the functionality to parse the ethernet, arp, ip, icmp, tcp, and udp headers. Finally, the remaining packet data gets printed out in ascii format where possible. The entirety of the program was written in C and was done individually.

### Takeaway
This project was super fun and help me to cement my understanding of the various packet protocols travelling across the internet. It was also my first time dealing with the network/host endianness issues and then splitting partial bits out of the 16/32 bit values being read out of my packet.
