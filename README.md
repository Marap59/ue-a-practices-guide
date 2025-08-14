# ue-a-practices-guide
Practices for efficient naming conventions, organized content structure, and readable Blueprint code.

# Premise
This guide is not meant to tell you how you must work, but to suggest how you _**might**_ work.
> Don’t have your own personal style? You’re welcome to try mine.\
> Already have one? That’s cool, feel free to read on anyway!

## Credits
Heavely inspired by [Allars's UE Style Guide](https://github.com/Allar/ue5-style-guide.git).

# Index
> [Content Structure](#1-Content-Structure)

> [Naming Convention](#2-Naming-Convention)

> [Blueprint Coding Practices](#3-Blueprint-Coding-Practices)  

# 1. Content Structure

## 1.1. Prerequisites
As soon as the project is created, make a folder inside the Content folder and **name** it after the **project**. From now on, we will work in that specific folder.

*Optional*: Add a ```Plugins``` folder inside the Content folder, where you can move any folders added by plugins

## 1.2. The Idea

The main idea is to make folders based on the type of **family** they are going to contain. With family I mean a group of assets that represents a category which may be: characters, weapons, vehicles, envirnoment for X city.

## 1.3. Generic Example

```
|--Content
  |--ProjectName
    |  |--Audio
    |  |  |--Metasound
    |  |  |--OST
    |  |  |--SFX
    |  |  |  |--Protagonist
    |  |  |  |--Metal Detector
    |  |  |  |--UI
    |  |--Characters
    |  |  |--Antagonist
    |  |  |--Assistant
    |  |  |--Protragonist
    |  |  |  |--Animations
    |  |  |  |--Blueprint (or Logic)
    |  |  |  |--Model
    |  |--Core
    |  |  |--Controls
    |  |  |--GameModes&Instances
    |  |  |--Utilities
    |  |  |  |--Data Tables
    |  |  |  |--Enumerators
    |  |  |  |--Function Libraries
    |  |  |  |--Interfaces
    |  |--Developers
    |  |--Maps
    |  |  |--City
    |  |  |--FinalLevel
    |  |  |--Lobby
    |  |  |  |--Interactive Assets
    |  |  |  |--Non_Interactive Assets
    |  |--Tools
    |  |  |--Bucket
    |  |  |--Metal Detector
    |  |  |--Shovel
    |  |--UI
    |  |  |--Assets
    |  |  |  |--Generic
    |  |  |  |--HUD
    |  |  |  |--MainMenu
    |  |  |--Blueprint
    |  |  |  |--Generic
```

|Name|Explanation|
|--|--|
|**Audio**|Collection of any type of audio asset. From soundtracks to generic or specific SFXs to Metasound and so on|
|**Characters**|Collection of NPCs and playable characters. Each has it's own folder and inside there are every type of asset related to that character|
|**Core**|Folders exclusively for programmers. Contains exclusively assets useful for programming stuff|
|**Developers**|Programmers chance to throw anything there and not to follow any rule|
|**Maps**|Each Map/Level has its own folder. Inside it there are also all the assets relative to that map, grouped by Interactive and Non-Interactive assets|
|**Tools**|Same as `Characters` but for playable tools. Same can be made for `Weapons` for example|
|**UI**|Same as `Audio` but for assets relative to UI. E.g. WBP, UI textures, videos.|

# 2. Naming Convention

## 2.1. Base Asset Name
`Prefix_BaseAssetName_Variant_Suffix`\
\
`BaseAssetName` should be simple and recognizible as well as the `Variant` if present.
For generic assets, use **digits** as `Variant`.\
\
Examples:
- BP_Shovel_Broken;
- T_Umbrella_01_BC.

## 2.2. Asset Name Modifiers

Credits to [Starforge Games](https://github.com/StarforgeGames/UE-Style-Guide.git) for most of the suffixes and, more importantly, for reminding me of the many different types of assets.

### Sections

> 2.2.1. [Animations](#221-animations)

> 2.2.2. [Artificial Intelligence](#222-artificial-intelligence)

> 2.2.3. [Blueprints](#223-blueprints)

> 2.2.4. [Materials](#224-materials)

> 2.2.5. [Texture](#225-texture)

> 2.2.6. [Miscellaneous](#226-miscellaneous)

> 2.2.7. [Paper 2D](#227-paper-2d)

> 2.2.8. [Physics](#228-physics)

> 2.2.9. [Sounds](#229-sounds)

> 2.2.10. [User Interface](#2210-user-interface)

> 2.2.11. [Effects](#2211-effects)

> 2.2.12. [Input](#2212-input)

### 2.2.1 Animations

|Asset Type|Prefix|Suffix|Notes|
|--|--|--|--|
|Aim Offset|AO|||
|Animation Blueprint|ABP|||
|Animation Composite|AC|||
|Animation Montage|AM|||
|Animation Sequence|AS|||
|Blend Space|BS|||
|Level Sequence|LS|||
|Morph Target|MT|||
|Paper Flipbook|PFb|||
|Rig|Rig|||
|Control Rig|CR|||
|Skeletal Mesh|SK|||
|Skeleton|SKEL|||

### 2.2.2. Artificial Intelligence

|Asset Type|Prefix|Suffix|Notes|
|--|--|--|--|
|AI Controller|AIC|||
|Behavior Tree|BT|||
|Blackboard|BB|||
|Decorator|BT|Decorator||
|Service|BT|Service||
|Task|BT|Task||
|Environment Query|EQS|||
|EnvQueryContext|EQS|Context||

### 2.2.3. Blueprints

|Asset Type|Prefix|Suffix|Notes|
|--|--|--|--|
|Blueprint|BP|||
|Blueprint Component|BP|Component||
|Blueprint Function Library|BPFL|||
|Blueprint Interface|BPI|||
|Blueprint Macro Library|BPML|||
|Enumeration|E||NO UNDERSCORE|
|Structure|S||NO UNDERSCORE|
|Tutorial Blueprint|TBP|||
|Widget Blueprint|WBP|||

### 2.2.4. Materials

|Asset Type|Prefix|Suffix|Notes|
|--|--|--|--|
|Material|M|||
|Material (Post Process)|PP|||
|Material Function|MF|||
|Material Instance|MI|||
|Material Parameter Collection|MPC|||
|Subsurface Profile|SP|||
|Physical Materials|PM|||
|Decal|MD|||

### 2.2.5. Texture

|Asset Type|Prefix|Suffix|Notes|
|--|--|--|--|
|Texture|T|||
|Diffuse/Albedo/Base Color|T|BC||
|Metallic|T|M||
|Normal|T|N||
|Roughness|T|R||
|Alpha/Opacity|T|A||
|Ambient Occlusion|T|AO||
|Bump|T|B||
|Emissive|T|E||
|Mask|T|M||
|Specular|T|S||
|Displacement|T|DP||
|Texture Cube|TC|||
|Media Texture|MT|||
|Render Target|RT|||
|Cube Render Target|RT|||
|Texture Light Profile|TLP|||

For textures that include multiple layers of texture data, _it is common to stack the suffixes together into one_. There’s no strict ideal order to follow, so I recommend deciding on a consistent style in advance. If you’re working with a team, be sure to discuss and agree on this order together.

### 2.2.6. Miscellaneous

|Asset Type|Prefix|Suffix|Notes|
|--|--|--|--|
|Animated Vector Field|VFA|||
|Camera Anim|Ca|||
|Color Curve|Curve|Color||
|Curve Table|Curve|Table||
|Data Table|DT|||
|Float Curve|Curve|Float||
|Foliage Type|FT|||
|Landscape Grass Type|LG|||
|Landscape Layer|LL|||
|Level/Map|L|||
|Level (Persistent)|L|P||
|Level (Audio)|L|Audio||
|Level (Lighting)|L|Light||
|Level (Geometry)|L|Geo||
|Level (Gameplay)|L|Gameplay||
|Matinee Data||Matinee||
|Media Player|MP|||
|File Media Source|FMS|||
|Object Library|OL|||
|Sprite Sheet|SS|||
|Static Mesh|SM|||
|Static Vector Field|VF|||
|Substance Graphs Instance|SGI|||
|Substance Instance Factory|SIF|||
|Touch Interface Setup|TI|||
|Vector Curve|Curve|Vector||

### 2.2.7. Paper 2D

|Asset Type|Prefix|Suffix|Notes|
|--|--|--|--|
|Paper Flipbook|PFb|||
|Sprite|SPR|||
|Sprite Atlas Group|SPRG|||
|Tile Map|TM|||
|Tile Set|TS|||

### 2.2.8. Physics

|Asset Type|Prefix|Suffix|Notes|
|--|--|--|--|
|Physical Material|PM|||
|Physical Asset|PHYS|||
|Destructible Mesh|DM|||

### 2.2.9. Sounds

|Asset Type|Prefix|Suffix|Notes|
|--|--|--|--|
|Dialogue Voice|DV|||
|Dialogue Wave|DW|||
|Media Sound Wave|MSW|||
|Reverb Effect|Rvb|||
|Sound Attenuation|S|Att||
|Sound Class|||No prefix/suffix. Should be put in a folder called ```SoundClasses```|
|Sound Concurrency|SC||Should be named after a SoundClass|
|Sound Cue|S|Cue||
|Sound Mix|S|Mix||
|Sound Wave|S|||
|MetaSound Source|MS|S|
|MetaSound Patch|MS|P||

### 2.2.10. User Interface

|Asset Type|Prefix|Suffix|Notes|
|--|--|--|--|
|Font|Fnt|||
|Slate Brush|Brsh|||
|Slate Widget Style|Stl|||
|Widget Blueprint|WBP|||

### 2.2.11. Effects

|Asset Type|Prefix|Suffix|Notes|
|--|--|--|--|
|Material (Post Process)|PP|||
|Niagara Emitter|N|E||
|Niagara System|N|S||
|Niagara Module|N|M||
|Niagara Dynamic Input Script|N|IS||
|Niagara Function Script|N|FS||
|Niagara Module Script|N|MS||
|Niagara Data Channel|N|DC||
|Niagara Effect Type|N|ET||
|Niagara Parameter Collection|N|P||
|Niagara Parameter Collection Instance|N|PI||
|Niagara Parameter Definitions|N|PD||
|Niagara Simulation Cache|N|SC||
|Niagara Validation Rule Set|N|VRS||

### 2.2.12. Input

|Asset Type|Prefix|Suffix|Notes|
|--|--|--|--|
|Input Mapping Context|IMC|||
|Input Action|IA|||
|Force Feedback Attenuation|FFA|||
|Force Feedback Effect|FFE|||

# 3. Blueprint Coding Practices

When writing code, it is essential to keep it **clean and readable** while minimizing dependencies. This increases modularity and makes it easier for others to work with the code, both now and in the future.\
In this section of the guide, I will discuss practices specific to Blueprints, focusing in particular on how and when to use Events, Comments, Collapsed Nodes, Functions, and Macros.

## Sections

> 3.1. [Collapsed Nodes and Comments](#31-Collapsed-Nodes-and-Comments)

> 3.2. [Functions and Macros](#32-Functions-and-Macros)

> 3.3. [Custom Events](#33-Custom-Events)

## 3.1. Collapsed Nodes and Comments

It is common to use comments to group portions of code, ranging from small to more extensive segments, while describing their logic. This is a very useful practice, but depending on the complexity of the Blueprint (BP), there is a risk of ending up overwhelmed by a considerable amount of code, further cluttered by numerous comments. Unless you are a programmer used to working in the dark, the overall view can become quite distracting, as it is not immediately clear what to look at or where to focus first.\
In my case, I use comments exclusively to group related pieces of logic that belong to the same functional category, providing in a few words an identifying label for each group.

|Example|
|--|
|The events related to **graphic** settings are all grouped under a single comment, just as those for **audio** and **input** settings are. Once they are divided into these specific categories, I add another overarching comment that encloses them all, since they are part of a broader group: the events related to **settings**.|

Colors, on the other hand, are very useful for improving visual clarity, especially when the same color is used across multiple Blueprints to identify the same category or type of event.

|Example|
|--|
|Use green for common events such as Begin Play and Construct.|
|Use red for Event Tick.|
|Use yellow for Enhanced Input events.|

So far, we have seen how to organize code based on logical categories, but there is still the need to describe certain sequences of nodes in more detail. To address this, I make extensive use of the **Collapse Nodes** feature.\
This proves extremely effective for keeping the graph clean and improving overall readability, even at a glance.\
As with comments, I group nodes according to a logical criterion; however, when necessary, the name assigned to the collapsed node will be more descriptive than the concise labels used in comments.

|Example|
|--|
|![](/images/bp-practices/cn-example-01.jpg)In this first image, we can see a main group named `Main Logic`, inside which there are two Collapsed Graphs. If, upon opening the BP, I needed to locate the logic related to `Scale`, knowing that it is part of the main logic, I would already know to look inside `Main Logic`. At that point, I would immediately find the Collapsed Graph named `Move and Scale`, which would contain exactly what I was looking for.|
|![](/images/bp-practices/cn-example-02.jpg)The second image demonstrates how it is possible to group logic in a way that allows you to directly identify the part of interest, avoiding the need to scroll horizontally through the nodes.|

## 3.2. Functions and Macros

To proceed, it is key to comprehend  what a function is and what it can do:
> _Functions are node graphs belonging to a particular Blueprint that can be executed, or called, from another graph within the Blueprint._
> Source: [UE Documentation](https://dev.epicgames.com/documentation/en-us/unreal-engine/functions-in-unreal-engine)

From this definition, we can understand that functions have the characteristic of being callable whenever needed. Based on this premise, I will write functions only in the following cases:

- Whenever I need a function like to trigger an event at a specific point in the game, or to allow a third-party actor with a reference to the function’s owner to call it.
- When I need to repeat the same logic multiple times, avoiding duplicated code, I can use a function. In this case, the function becomes part of a library of useful, reusable logic, which Unreal Engine allows you to access quickly through a dedicated window.

Macros, like functions, are designed to speed up and simplify programming by avoiding duplicated code and making reusable logic available at any time. Macros can also be easily called through the dedicated window in Unreal Engine.
However, unlike functions, macros are generally used for more practical and utilitarian logic.

|Examples||
|--|--|
|**Functions**|**Macros**|
|Load or Save settings' variables to a save slot|Conversion of a 2D struct to a custom text format|
|In an arcade racing game, generate and equip to a player a PowerUp when hitting a Box|Given as input an object, verify and output if it is valid based on specific checks|

## 3.3. Custom Events

Given the highly versatile nature of Custom Events—and events in general—I do not assign them a fixed role within my programming methodology. Excluding common events such as `Tick` and `BeginPlay`, or precompiled ones associated with specific classes, such as `BeginOverlap` for collision components, I will mainly use Custom Events when I need to handle logic containing latent nodes or when it is necessary to implement binding logic.\
It is important to note that events offer many more possibilities than those mentioned here, but exploring them in detail goes beyond the scope of this guide.


