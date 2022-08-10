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

* Dolphin
* Smalltalk MT
* Squeak VMs
* * Cog/OpenSmalltalkVM
* * RoarVM
* * SqueakJS
* * RSqueak
* * TruffleSqueak
* * JSqueak/Potato
* * Jitter
* * Jitter3
* * Jitter5
* Cuis
* Pharo
* Bee Smalltalk
* PigeonTalk
* Smalltalk 25
* Object Studio
* Smalltalk V/DOS 2
* Smalltalk V/Win
* Smalltalk V/Mac
* Smalltalk V/PM
* VisualWorks
* LST forks
* * SmallWorld
* * SmallWorld 2007
* * PDST
* * Susie
* * Parla
* * LST 4.5
* * ATalk
* * Tumbleweed
* SmalltalkAgents
* S#
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
* Haver on Cuis
* Huemul


### Initial Release

| year | name and version    | type     | authors                       | license    | description |
|------|---------------------|----------|-------------------------------|------------|-------------|
| 2015 | Spry                | system   | Göran Krampe                  | open       | very tiny but Smalltalk-like implemented in Nim |
| 2012 | Mist                | system   | Martin McClure                | open       | simple Smalltalk-in-Smalltalk that compiles to x86-64 |
| 2011 | Amber Smalltalk     | system   | Nicolas Petton                | open       | runs on Javascript |
| 2010 | Sly                 | image    | David Ungar, Sam Adams        | open       | extends Squeak to implement ensembles and adverbs on the RoarVM |
| 2003 | GNU Smalltalk       | system   | Steve Byrne, Paolo Bonzini    | open       | text based |
| 2002 | OOVM                | system   | Lars Bak                      | commercial | Smalltalk for embedded devices, with special block arguments |
| 2002 | Slate               | system   | Lee Salzman, Brian Rice       | open       | prototype based with multiple dispatch |
| 2000 | Bistro              | system   | Nik Boyd                      | open       | Smalltalk on top of the Java VM |
| 1999 | F-Script            | system   | Philippe Mougin               | open       | Smalltalk layer on top of Cocoa MacOS, with APL style extensions |
| 1998 | Pocket Smalltlk     | system   | Andrew Brault                 | open       | develop in an IDE an generate executable for Palm Pilot |
| 1996 | Squeak              | system   | Apple                         | open       | VM written in Slang (Smalltalk subset) and simulated within Smalltalk |
| 1996 | Strongtalk          | system   | Animorphic Systems            | commercial | vm techniques from Self, optional typing, traits |
| 1993 | VisualAge           | system   | IBM                           | commercial | focus on IDE for various languages |
| 1988 | ConcurrentSmalltalk | hardware | MIT                           | internal   | Lisp syntax version of Smalltalk on the 1024 processor J-Machine |
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
| 1984 | Clone/Reduce        | vm       | Jecel Assumpção Jr            | open       | An alternative execution model via copying ASTs at runtime |
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

### Further Releases and Forks

| year | name and version    | authors                       | license    | description |
|------|---------------------|-------------------------------|------------|-------------|
| 2022 | Squeak 6.0          | Squeak Board                  | open       | high resolution, uses SistaV1 bytecodes |
| 2015 | Squeak 5.0          | Squeak Board                  | open       | introduced Spur memory model |
| 2008 | Squeak 3.10         | Squeak Board                  | open       | first release after Pharo fork |
| 2007 | Little Smalltalk 5  | Charles Childers              | open       |             |
| 2006 | Strongtalk          | Sun                           | open       | an open source release of the vm from the 1997 Strongtalk |
| 2005 | Little Smalltalk 4  | Tim Budd                      | open       | metaclasses, compiler in Smalltalk |            |
| 2002 | Strongtalk          | Sun                           | open       | an open source release of the image from the 1997 Strongtalk |
| 2001 | Squeak 3.0          | Squeak Central                | open       | switched to Morphic as default GUI |
| 2000 | Squeak 2.0          | Squeak Central                | open       | pluggable views, Morphic |
| 1994 | Smalltalk/X         | eXept Software AG             | open       | moved from hobby to commercial development |
| 1990 | Smalltalk/X         | Claus Gittinger               |            | added JIT compilation |
| 1988 | Smalltalk/X         | Claus Gittinger               | internal   | added bytecode interpreter |
| 1988 | Little Smalltalk 3  | Tim Budd                      | open       | reorganized source tree |
| 1987 | Little Smalltalk 2  | Tim Budd                      | open       | globals, more code moved to Smalltalk |
