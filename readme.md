# About

GLfo is a live video performance framework for the Pure Data/GEM programming language.

# Goals

GLfo aims to provide a comprehensive set of modulation sources useful for creating
interactive visual instruments. It also provides a framework for composing several 
scenes together into a live video performance set. 

# Requirements

GLfo is being tested under Pure Data Extended with the included GEM libraries. 
It is tested occasionally on PC versions of PD.

# Usage

Run live-set.pd with Pure Data to see a simple sample set.

# Installing

Clone the GLfo repository and add the path to the PD search paths.

# Concepts

There are three basic concepts that GLfo relies on:

* Sets
* Scenes
* Presets

## Sets

A set in GLfo is a collection of scenes. A set is designed to be a unit of performance. The set is loaded
at the beginning of the performance and is used to launch the rest of the scenes in the performance.

## Scenes

A scene is a segment of a set that can be transitioned to or from. A scene is a self-contained OpenGL rendering
chain that is rendered ultimately to a framebuffer, where the set can project the framebuffer as a texture
onto a scene card (for instance).


## Presets

A preset is simply a collection of values that store the state of a scene. Many times a scene will have 
values that need to be initialized or can radically alter it once running. Presets give you a way to 
store and recall these states.

# Future

* Scene stacks
* Centralized preset management
* Animation between presets

