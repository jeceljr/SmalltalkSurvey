# SmalltalkSurvey

The goal is to compile a reasonably complete list of all implementations of the Smalltalk system.

![Hot air ballons form Wikipedia](images/1024px-Hot_air_balloons_in_leon.jpg)

### What is Smalltalk?

A language will be considered to be a Smalltalk (1) if it is easy to type in an example from a Smalltalk-80 book while adapting it on the fly (not counting any differences in the libraries) or (2) if "smalltalk" is part of the project's name.

Rule 1 is very subjective. For some people it might be trivial to translate Smalltalk-80 into Objective-C or Javascript while typing at full speed, but many others would find it a bit complicated.

The reason for rule 2 is to allow an implementation's creators to decide. If they selected to include "smalltalk" in the name of their project then their intent should be respected. In the current version of the list below only Smalltalk-72 (and -74) and MIT's ConcurrentSmalltalk depend on this rule. It would be silly to exclude the very first Smalltalk even if it lacks many features that later became standard and the Lisp syntax of the MIT project is only a small issue given how the rest of the project adopts the traditional Smalltalk ideas.

### Type

"Paper" means that a description of the language was published without a corresponding implementation (at that time). "System" indicates that both a virtual machine and an image including libraries were implemented. "VM" means that a new virtual machine was created to run some existing image, while "image" indicates a new image and libraries running on a previously implemented virtual machine.

### License

"Open" means that the license is in the spirit of Open Source or Free Software. "Commercial" is closed software that was sold. "Internal" was not made available to the public at all. "No cost" was made available without payment but without the sources (the more proper term "freeware" would cause confusion with Free Software and so was avoided).

## Implementations:

To add:

* Dolphin
* Smalltalk MT
* Smalltalk/X
* Squeak VMs
* * Cog/OpenSmalltalkVM
* * RoarVM
* * SqueakJS
* * RSqueak
* * TruffleSqueak
* Cuis
* Pharo
* Bee Smalltalk
* MIST
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
* Haver on Cuis
* Huemul
* F-Script
* OPL-432
* Slate
* Pocket Smalltalk
* Bistro
* OOVM
* StrongTalk
* Berkeley Smalltalk
* Apple Smalltalk
* Tektronix Smalltalk
* DEC Smalltalk
* HP Smalltalk


| year | name and version | type | authors | license | description |
|------|------------------|------|---------|---------|-------------|
| 2011 | Amber Smalltalk | system | Nicolas Petton | open | runs on Javascript |
| 2003 | GNU Smalltalk | system | Steve Byrne and Paolo Bonzini | open | text based |
| 1996 | Squeak | system | Apple | open | VM written in Slang (Smalltalk subset) and simulated within Smalltalk |
| 1993 | VisualAge | system | IBM | commercial | focus on IDE for various languages |
| 1989 | Mushroom | hardware | Manchester | internal | multiple FPGAs |
| 1989 | ConcurrentSmalltalk | hardware | MIT | internal | Lisp syntax version of Smalltalk on the 1024 processor J-Machine |
| 1987 | Self         | paper  | Dave Ungar and Randy Smith |  | prototype based |
| 1986 | Smalltalk V  | system | Digitalk | commercial | graphic Smalltalk on DOS |
| 1986 | GemStone/S | system | Servio | commercial | integrated database and Smalltalk |
| 1985 | Methods      | system | Digitalk | commercial | text GUI on the IBM PC |
| 1985 | Smalltalk-PC | system | Christopher Made |    | implementation of the Apple II and other micros |
| 1984 | Little Smalltalk 1 | system | Tim Budd | open | text based for Unix machines with corresponding book |
| 1984 | Clone/Reduce | vm | Jecel Assumpcao Jr | open | An alternative execution model via copying ASTs at runtime |
| 1984 | SOAR | hardware | Berkeley | internal | Smalltalk On A RISC processor and software |
| 1980 | TinyTalk     | system | PARC | internal | 64KB adaptation of Smalltalk-76 |
| 1980 | Smalltalk-80 | system | PARC |   | release to the world |
| 1978 | Smalltalk-78 | system | PARC | internal | Notetaker |
| 1976 | Smalltalk-76 | system | PARC | internal | bytecodes and inheritance |
| 1972 | Smalltalk-72 | system | PARC | internal | first implementation |
| 1971 | Smalltalk-71 | paper | PARC |    | initial ideas
