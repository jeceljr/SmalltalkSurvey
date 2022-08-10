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

| year | name and version | type | authors | license | description |
|------|------------------|------|---------|---------|-------------|
| 1989 | ConcurrentSmalltalk | hardware | MIT | internal | Lisp syntax version of Smalltalk on the 1024 processor J-Machine |
| 1985 | Methods      | system | Digitalk | commercial | text GUI on the IBM PC |
|      | Little Smalltalk 1 | system | Tim | open | text based for Unix machines with corresponding book |
| 1984 | Clone/Reduce | vm | Jecel | open | An alternative execution model via copying ASTs at runtime |
|      | TinyTalk     | system | PARC | internal | 64KB adaptation of Smalltalk-76 |
| 1980 | Smalltalk-80 | system | PARC |   | release to the world |
| 1978 | Smalltalk-78 | system | PARC | internal | Notetaker |
| 1976 | Smalltalk-76 | system | PARC | internal | bytecodes and inheritance |
| 1972 | Smalltalk-72 | system | PARC | internal | first implementation |
| 1971 | Smalltalk-71 | paper | PARC |    | initial ideas
