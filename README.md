# SmalltalkSurvey

The goal is to compile a reasonably complete list of all implementations of the Smalltalk system.

![Hot air ballons form Wikipedia](images/1024px-Hot_air_balloons_in_leon.jpg)

While it is very common for a recent language to have a single, open source implementation thanks to the Internet and to the reduced kinds of computers now available, it used to be inevitable for interesting languages to have many different implementations. The most common reason was due to the language not being available on your computer, or only a very expensive commercial version being available. The languages themselves were simpler and didn't include much in terms of libraries, so the effort to implement from a written description was not too bad. These descriptions were often not complete, leaving the implementors to guess many details and to include their own ideas. While languages like Basic and Pascal split into many dialects, the Forth, Lisp and Smalltalk communities were specially prone to this.

This page tries to trace the many Smalltalk dialects created over the years. In theory the separation of the system into a virtual machine running an "image" file should have helped splits be less common than in other languages, but in practice commercial reasons and hardware limitations encouraged recreating the image from scratch in many different projects.

### What is Smalltalk?

A language will be considered to be a Smalltalk if

1. it is easy to type in an example from a Smalltalk-80 book while adapting it on the fly (not counting any differences in the libraries) or
2. if "smalltalk" is part of the project's name.

Rule 1 is very subjective. For some people it might be trivial to translate Smalltalk-80 into Objective-C or Javascript while typing at full speed, but many others would find it a bit complicated.

The reason for rule 2 is to allow an implementation's creators to decide. If they selected to include "smalltalk" in the name of their project then their intent should be respected. In the current version of the list below only Smalltalk-72 (and -74) and MIT's ConcurrentSmalltalk depend on this rule. It would be silly to exclude the very first Smalltalk even if it lacks many features that later became standard and the Lisp syntax of the MIT project is only a small issue given how the rest of the project adopts the traditional Smalltalk ideas.

### Type

"Paper" means that a description of the language was published without a corresponding implementation (at that time). "System" indicates that both a virtual machine and an image including libraries were implemented. "VM" means that a new virtual machine was created to run some existing image, while "image" indicates a new image and libraries running on a previously implemented virtual machine or an implemention on top of an existing system.

### License

"Open" means that the license is in the spirit of Open Source or Free Software. "Commercial" is closed software that was sold. "Internal" was not made available to the public at all. "No cost" was made available without payment but without the sources (the more proper term "freeware" would cause confusion with Free Software and so was avoided).

## Implementations:

To add:

* LST forks
* * SmallWorld
* * SmallWorld 2007
* * PDST
* * Susie
* * Parla
* * LST 4.5
* * ATalk
* * Tumbleweed
* Self derived
* * Self4Linux
* * tinySelf 1
* * Klein
* * Us
* * Korz
* * JSelf
* * DSelf
* * OpenSelf
* * Self/R
* Squeak VMs
* * SqueakJS
* * RSqueak
* * JSqueak/Potato
* * Jitter
* * Jitter3
* * Jitter5

Taken from [a draft Smalltalk history at Simberon](http://simberon.blogspot.com/2012/04/smalltalk-history-draft-2.html):
![relationship between Smalltalk implementations](./images/SmalltalkHistory.png)

### Initial Release and Forks

| year | name and version    | type     | authors                       | license    | description |
|------|---------------------|----------|-------------------------------|------------|-------------|
| 2022 | PigeonTalk          | system   | David Buck                    |            | block based, like Scratch  |
| 2021 | Zag                 | system   | David Mason                   | open       | VM written in Zig |
| 2020 | Haver               | image    | Gerald Klix                   | open       | runs on Cuis and adds modules |
| 2020 | Crosstalk           | vm       | Michael Engel                 | [open](https://github.com/michaelengel/crosstalk) | Smalltalk-80 VM in C++ for Raspberry Pi |
| 2020 | Smalltalk           | vm       | Dan Banay                     | [open](https://github.com/dbanay/Smalltalk) | translations of the "Blue Book" VM to C |
| 2020 | Smalltalk           | vm       | Rochus Keller                 | [open](https://github.com/rochus-keller/Smalltalk) | interpreter and other tools to explore the orignal Smalltalk-80 image |
| 2017 | TruffleSqueak       | vm       | Hasso PLattner Institut       | [open](https://github.com/hpi-swa/trufflesqueak) | uses Truffle and GraalVM |
| 2015 | Spry                | system   | Göran Krampe                  | [open](https://github.com/gokr/spry)       | very tiny but Smalltalk-like implemented in Nim |
| 2014 | Smalltalk 25        | system   | Boris Shingarov               |            | generate a VM from the definition of a processor |
| 2014 | Bee Smalltalk       | system   | Javier Pimás, Javier Burroni, Gerardo Richarte | open      | metacircular Smalltalk            |
| 2012 | Mist                | system   | Martin McClure                | open       | simple Smalltalk-in-Smalltalk that compiles to x86-64 |
| 2011 | Amber Smalltalk     | system   | Nicolas Petton                | [open](https://github.com/amber-smalltalk/amber)      | runs on Javascript |
| 2011 | Redline Smalltalk   | system   | James Ladd, Sean Allen        | [open](https://github.com/redline-smalltalk/redline-smalltalk)       | runs on the Java VM |
| 2011 | Objective-Smalltalk | system   | Marcel Weiher                 | [open](https://github.com/mpw/Objective-Smalltalk) | combines features from Objective-C and Smalltalk |
| 2010 | Sly                 | image    | David Ungar, Sam Adams        | open       | extends Squeak to implement ensembles and adverbs on the RoarVM |
| 2010 | Pinocchio           | system   | U of Berne                    | open       | meta-circular VM |
| 2009 | Cuis 1.0            | image    | Juan Vuletich                 | [open](https://github.com/Cuis-Smalltalk/Cuis-Smalltalk-Dev)       | fork of Squeak 3.7 to make it simpler |
| 2009 | Pharo 0.1           | image    | Pharo Board                   | [open](https://github.com/pharo-project/pharo)       | fork of Squeak 3.9 to go in a different direction |
| 2008 | RoarVM              | vm       | David Ungar, Sam Adams        | [open](https://github.com/smarr/RoarVM) | a rewrite of the SqueakVM in C++ to run on manycore machines |
| 2008  | OpenSmalltalkVM    | vm       | Eliot Miranda                 | [open](https://github.com/OpenSmalltalk/opensmalltalk-vm) | fork of the SqueakVM to do JIT compilation and other enhancements |
| 2008 | Huemul              | system   | Guilleromo Adirán Molina      |            | uses Exupery to compile to x86 |
| 2002 | #Smalltalk          | system   | John Brant, Don Roberts       | open       | Smalltalk for .NET |
| 2002 | OOVM                | system   | Lars Bak                      | commercial | Smalltalk for embedded devices, with special block arguments |
| 2002 | Slate               | system   | Lee Salzman, Brian Rice       | [open](https://github.com/briantrice/slate-language)     | prototype based with multiple dispatch |
| 2002 | S#                  | system   | David Simmons                 | commercial | Smalltalk for .NET |
| 2002 | SOM                 | system   | U of Aarhus                   | open       | SimpleObjectMachine for teaching implementation techniques |
| 2001 | LSWVST              | system   | Lesser-Software               | commercial | bytecode compatible with Smalltalk/V |
| 2000 | Bistro              | system   | Nik Boyd                      | open       | Smalltalk on top of the Java VM |
| 1999 | F-Script            | system   | Philippe Mougin               | open       | Smalltalk layer on top of Cocoa MacOS, with APL style extensions |
| 1998 | Dolphin             | system   | Object Arts                   | commercial | small system optimized for Windows |
| 1998 | Pocket Smalltlk     | system   | Andrew Brault                 | open       | develop in an IDE an generate executable for Palm Pilot |
| 1996 | Squeak              | system   | Apple                         | open       | VM written in Slang (Smalltalk subset) and simulated within Smalltalk |
| 1996 | Strongtalk          | system   | Animorphic Systems            | commercial | vm techniques from Self, optional typing, traits |
| 1994 | Smalltalk MT        | system   | Tarik Kerroum                 | commercial | compiles Smalltalk to machine code with easy access to DLLs |
| 1994 | SmalltalkAgents     | system   | Quasar Knowledge Systems      | commercial | features optimized to access MacOS resources |
| 1993 | VisualAge           | system   | IBM                           | commercial | focus on IDE for various languages |
| 1990 | GNU Smalltalk       | system   | Steve Byrne, Paolo Bonzini    | open       | text based |
| 1989 | Object Studio       | system   | ENFIN                         | commercial | originally called SCOPE, for military applications on the PC |
| 1988 | ConcurrentSmalltalk | hardware | MIT                           | internal   | Lisp syntax version of Smalltalk on the 1024 processor J-Machine |
| 1987 | VisualWorks         | system   | ParcPlace                     | commercial | spinoff from Xerox PARC to implement Smalltalk-80 for workstations (originally ObjectWorks) |
| 1987 | Mushroom            | hardware | U Manchester                  | internal   | multiple FPGAs and TTLs |
| 1987 | Self                | paper    | Dave Ungar, Randy Smith       |            | prototype based |
| 1986 | Smalltalk/X         | system   | Claus Gittinger               | internal   | Smalltalk to C translator, initially |
| 1986 | ConcurrentSmalltalk | system   | Yasuhiko Yokote, Mario Tokoro |            | implements "return and continue", mailboxes |
| 1986 | Swamp               | hardware | U Toronto                     | internal   | bitslice |
| 1986 | AI32                | hardware | Hitachi                       | internal   | chip |
| 1986 | Smalltalk V         | system   | Digitalk                      | commercial | graphic Smalltalk on DOS |
| 1986 | GemStone/S          | system   | Servio                        | commercial | integrated database and Smalltalk |
| 1985 | Methods             | system   | Digitalk                      | commercial | text GUI on the IBM PC |
| 1985 | Smalltalk-PC        | system   | Christopher Made              |            | implementation for the Apple II and other micros |
| 1984 | Sword32             | hardware | U Tokyo                       | internal   | chip |
| 1984 | COM                 | hardware | Caltech                       | internal   | Object architecture |
| 1984 | Little Smalltalk 1  | system   | Tim Budd                      | open       | text based for Unix machines with corresponding book |
| 1984 | Clone/Reduce        | vm       | Jecel Assumpção Jr            | internal   | An alternative execution model via copying ASTs at runtime |
| 1983 | SOAR                | hardware | Berkeley                      | internal   | Smalltalk On A RISC processor and software|
| 1981 | Smalltalk-80        | vm       | Tektronix                     | internal   | 68000 prototype |
| 1981 | Smalltalk-80        | vm       | Apple                         | internal   | Lisa |
| 1981 | Smalltalk-80        | vm       | DEC                           | internal   | 32 bit port to the VAX |
| 1981 | Smalltalk-80        | vm       | HP                            | internal   | VAX |
| 1981 | Smalltalk-80        | vm       | U Berkeley                    |            | VAX |
| 1981 | OPL 432             | system   | Scott Warren                  | commercial | port of Rosetta Smalltalk to Intel's iAPX432 system |
| 1981 | Rosetta Smalltalk   | system   | Scott Warren                  |            | for 8 bit microcomputers, shown at the Exidy booth at NCC'81 | 
| 1980 | TinyTalk            | system   | PARC                          | internal   | 64KB adaptation of Smalltalk-76 |
| 1980 | Smalltalk-80        | system   | PARC                          |            | release to the world |
| 1978 | Smalltalk-78        | system   | PARC                          | internal   | Notetaker |
| 1976 | Smalltalk-76        | system   | PARC                          | internal   | bytecodes and inheritance |
| 1974 | Smalltalk-74        | system   | PARC                          | internal   | OOZE (object-oriented zoned environment) virtual memory system |
| 1972 | Smalltalk-72        | system   | PARC                          | internal   | first implementation |
| 1971 | Smalltalk-71        | paper    | PARC                          |            | initial ideas

### Further Major Releases

| year | name and version    | authors                       | license    | description |
|------|---------------------|-------------------------------|------------|-------------|
| 2022 | Squeak 6.0          | Squeak Board                  | open       | high resolution, uses SistaV1 bytecodes |
| 2022 | Cuis 6              | Juan Vuletich                 | open       | includes Morphic 3 |
| 2022 | VAST Platform 11.0.0| Instanciations                | commercial |             |
| 2022 | Pharo 10            | Pharo Board                   | open       |             |
| 2021 | VAST Platform 10.0.0| Instanciations                | commercial | renamed VA Smalltalk to VAST Platform |
| 2021 | Pharo 9             | Pharo Board                   | commercial |             |
| 2020 | ObjectStudio 9.0    | Cincom                        | commercial |             |
| 2020 | VisualWorks 9.0     | Cincom                        | commercial |             |
| 2020 | Pharo 8.0           | Pharo Board                   | open       |             |
| 2019 | Pharo 7.0           | Pharo Board                   | open       |             |
| 2017 | VA Smalltalk 9.0    | Instanciations                | commercial |             |
| 2017 | Pharo 6.0           | Pharo Board                   | open       |             |
| 2016 | Cuis 5.0            | Juan Vuletich                 | open       |             |
| 2016 | Dolphin 7           | Object Arts                   | [open](https://github.com/dolphinsmalltalk/Dolphin)       | open sourced the system |
| 2016 | Pharo 5.0           | Pharo Board                   | open       |             |
| 2015 | Squeak 5.0          | Squeak Board                  | open       | introduced Spur memory model |
| 2015 | Pharo 4.0           | Pharo Board                   | open       |             |
| 2014 | Pharo 3.0           | Pharo Board                   | open       |             |
| 2014 | VisualWorks 8.0     | Cincom                        | commercial |             |
| 2013 | Pharo 2.0           | Pharo Board                   | open       |             |
| 2012 | Cuis 4.0            | Juan Vuletich                 | open       | better package support |
| 2011 | Cuis 3.0            | Juan Vuletich                 | open       | new look |
| 2010 | Cuis 2.0            | Juan Vuletich                 | open       | closure enabled, can used Co VM |
| 2009 | Pharo 1.0           | Pharo Board                   | open       |             |
| 2009 | VA Smalltalk 8.0    | Instanciations                | commercial |             |
| 2009 | Dolphin 6           | Object-Arts, Lesser Software  | commercial | moved Dolphin to LSWVST virtual machine |
| 2008 | Squeak 3.10         | Squeak Board                  | open       | first release after Pharo fork |
| 2007 | Little Smalltalk 5  | Charles Childers              | open       |             |
| 2006 | Strongtalk          | Sun                           | open       | an open source release of the vm from the 1997 Strongtalk |
| 2005 | Little Smalltalk 4  | Tim Budd                      | open       | metaclasses, compiler in Smalltalk |
| 2005 | VA Smalltalk 6.0.2  | Instanciations                | commercial | transition from IBM VisualAge to VA Smalltalk |
| 2002 | Strongtalk          | Sun                           | open       | an open source release of the image from the 1997 Strongtalk |
| 2002 | VisualWorks 7.0     | Cincom                        | commercial |             |
| 2001 | Squeak 3.0          | Squeak Central                | open       | switched to Morphic as default GUI |
| 2000 | Squeak 2.0          | Squeak Central                | open       | pluggable views, Morphic |
| 1999 | VisualWorks 5i      | Cincom                        | commercial | uses native stack |
| 1998 | VisualWorks 3.0     | ObjectShare                   | commercial |             |
| 1996 | Smalltalk Express   | ObjectShare                   | no cost    | freeware version of Smalltalk V/Win |
| 1995 | Visual Smalltalk 3.0| Digitalk                      | commercial | client and Enterprise versions for OS/2 and Windows NT |
| 1994 | Smalltalk/X         | eXept Software AG             | open       | moved from hobby to commercial development |
| 1994 | VisualWorks 3.0     | ParcPlace                     | commercial | enhanced database communication |
| 1991 | Smalltalk V/Win 3.0 | Digitalk                      | commercial |             |
| 1990 | Smalltalk/X         | Claus Gittinger               |            | added JIT compilation |
| 1988 | Smalltalk V/286     | Digitalk                      | commercial | protected mode system |
| 1988 | Smalltalk V 2.0     | Digitalk                      | commercial |             |
| 1988 | Smalltalk/X         | Claus Gittinger               | internal   | added bytecode interpreter |
| 1988 | Little Smalltalk 3  | Tim Budd                      | open       | reorganized source tree |
| 1987 | Little Smalltalk 2  | Tim Budd                      | open       | globals, more code moved to Smalltalk |
