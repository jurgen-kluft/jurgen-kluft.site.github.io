---
title: "Project Experience - Virtuos Games"
date: 2024-09-09
tags: ["resume", "experience", "software-engineering"]
categories: ["resume"]
description: ""
draft: false
---

Developing; Texture Upscale Pipeline
CODA (UE4) Co-development for Xbox One/Xbox Series, PS4/PS5, Nintendo Switch (2020-2022)
Unannounced Xbox/PS4 game (Proprietary Engine) Remaster (Xbox One, PS4) 2018-2019
Evaluating; Popcorn FX middleware 2018
L.A. Noire (Xbox 360 to Nintendo Switch) 2016-2017
Assassin’s Creed The Ezio Collection (PS4, XBox One) 2016-2016
Heavy Rain (PS3 to PS4 port, proprietary engine and tools) 2015-2016
Batman: Return to Arkham (PS4, Xbox One, PC, Unreal Engine 4) 2014-2016
Fable Anniversary (360, Unreal Engine 3) 2012-2013
MonsterJam: Path of Destruction (PS3, 360, Wii, PSP, NDS) 2010-2011
Motorstorm: Arctic Edge (PS2) 2009-2010
PMRII (PS2, NDS) 2008 - 2009
SpeedRacer (NDS) 2007 - 2008
Asphalt 2 (NDS) 2006-2007
StreetRiders (PSP) 2005-2006

## **Projects**

### Texture Upscale Pipeline 

Duration: ~4 months
Size: 2 Engineers
Platform; Windows PC

#### Virtuos Games

Technologies:
* C/C++, C#
* OpenSource upscalers:
    * ESRGAN (https://github.com/xinntao/Real-ESRGAN)
    * Waifu2x (https://github.com/nihui/waifu2x-ncnn-vulkan)
* Many image manipulation CLI tools written in C/C++:
    * tiling enlarge/shrink
    * alpha split/merge
    * smart blend
    * color correction
    * normal decode/renormalize
* Multi-Threaded
* Structured Logging
* Fully configurable upscale pipelines
* 
* Custom JSON deserialization
* Visual Studio 2022

### L.A. Noire (Xbox 360 to Nintendo Switch) (2015-2016)

Duration: ~11 months
Size: 10-15 Engineers
Title: Technical Director; working with 2 Lead Engineers, 6 Senior and 6 Junior Engineers
Platform: A PS3/Xbox-360 game porting to Nintendo Switch

#### Virtuos Games

Technologies:
* Umbra
* FMOD
* Xbox 360 / PS3 SDK
* Nintendo Switch SDK
* ARM NEON for optimizing Math (https://en.wikipedia.org/wiki/ARM_architecture#Advanced_SIMD_(NEON))
* Visual Studio 2015
* Incredibuild
* FramePro and MemPro

Tasks:

* Wrote runtime component to save profile and memory allocation events with stack-trace and scope, frame number and timing information from multiple threads
* Wrote a tool to convert the profile information to a format that could be read by FramePro
* Wrote a GPU memory allocator based on best-fit algorithm
* Integrated UMBRA into the data building pipeline and runtime
* Part of the realtime MPG streams where converted to use Bink to increase CPU performance
* Refactored a lot of global scope object instances to 'create on initialization'
* Made the decision and changes to have all streaming data uncompressed to increase CPU performance
* Assisted Senior Engineer to analyze/profile file-IO to write an optimum FileReader
* Assisted Senior Engineer to port old FMOD-Ex to FMOD Studio for Nintendo Switch

### Assassin’s Creed The Ezio Collection (PS4, XBox One)

A port to the Playstation 4 and Xbox One

#### Virtuos Games

* Managing a team of 10+ engineers
* Extending the data building tools to support Xbox One Porting the runtime to Xbox One
* GPU Profiling and optimizations
* Constant Buffer usage optimization

### Heavy Rain (PS3 to PS4 port, proprietary engine and tools)

Porting Heavy Rain PS3 to PS4

#### Virtuos Games

* Replaced custom memory allocator with DLMalloc and refactored the whole code-base to use a standard memory allocation API. This allowed us to swap from a final allocator to a debug allocator very easily during development.
* Wrote the PS4 render engine and made many render passes multi- threaded
* Working with Artists and Graphics Engineer to integrate 'cubemap based environment lighting'
* Integrated Bink to provide us with movie frames in an asynchronous manner
* Wrote a lock-less JOB system used for multi-threading animation and render-passes
* Did a lot of CPU optimizations to get the game at 30+ FPS

### Batman: Return to Arkham (PS4, Xbox One, PC, Unreal Engine 4)

A challenging port by merging engines, UE3 and UE4 and moving to a PBR pipeline

#### Virtuos Games

* Setup many details on how to merge UE3 core engine into UE4
* Extended Mercurial (Hg) to be able to handle large amount of binary data
* Designed an Artist PBR workflow to automate and ease the validation of PBR assets

### Fable Anniversary (XBox 360, Unreal Engine 3)

A port of an XBox game to Xbox 360 using Unreal Engine 3 merged with the old game engine

#### Virtuos Games

* UE3
* WWise
* Merging UE3 and proprietary game engine
* Designed the interface layer between proprietary engine and UE3
* UE3 package analysis and re-distribution of objects to match story line
* FaceFX
* Wrote a batch convertor for Audio/Voice to Face FX animation for all supported languages
* Localization compression
* Scaleform

### Generator Rex: Agent of Providence (PS3, 360, Wii)

Full development of Generator Rex using a custom engine and tools

#### Virtuos Games

* PhysX
* Visual Scripting
* Cross platform custom engine Custom Editor
* Managing a team of 25 engineers FMOD

### MonsterJam: Path of Destruction (PS3, 360, Wii)

Full development writing a custom cross platform engine and tools

#### Virtuos Games

* Managing a team of 20+ engineers
* Integrated Bullet Physics
* Terrain collision was done in a custom 'grid' manner to speed up raycasts
* Full Particle System and Editor
* WII render engine and material system

### Motorstorm: Arctic Edge (PS2)

Co-development, responsible for the PS2 version of the game

#### Virtuos Games

* VU0/VU1 skinning job
* Adjust data-building pipeline to also build PS2 graphic data PS2 render-engine
* Did a lot of implementation and refactoring of the PS2 render engine
* Automated performance testing
* CI/CD using Team City
* Perforce

### Pimp My Ride: Street Racing (PS2, NDS)

Full development of a Pimp My Ride game for PS2 as well as Nintendo DS

#### Virtuos Games

* Re-used and extended the C# based data description and build pipeline.
* Support for the data-pipeline to be incremental, caching converted assets and using a dependency tree
* Big-file re-ordering based on file-order-access logged by the game
* Designed and assisted with the implementation of a UI authoring pipeline using Microsoft Blend

### SpeedRacer (NDS)

Full development, game engine, AI, Tools, UI framework and networking

#### Virtuos Games

* Designed and Implemented the (Render) Engine to run at 60 FPS
* Designed the technical aspects of the 3D track structure and how cars would drive/navigate
* Written a full C# based data description and build pipeline
* Worked with VFX artist to make all of the VFX just scaling effects instead of actual particle simulation
* Big-file and index-file generation

### Asphalt 2 for Nintendo DS

Porting of Asphalt 2 (N-Gage) to Nintendo DS (2006-2007)

#### Virtuos Games

* Ported Render Engine to Nintendo DS
* Optimized (the hell) out of the UI rendering to get 30 FPS Integrated distance based fade-in/fade-out

### Street Riders PSP

Porting of Street Riders PS2 to PSP (2005-2006)

#### Virtuos Games

* CodeWarrior, C/C++
* CI/CD, CruiseControl
* Wrote the complete Render Engine for PSP
* Extended data-building tools to write out PSP graphic and texture formats
* Optimized the skinned mesh parts (bone constraint) using minimum spanning trees
* Optimizations, C/C++

