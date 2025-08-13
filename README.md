# ue-a-practices-guide
Practices for efficient naming conventions, organized content structure, and readable Blueprint code.

# Premise
This guide is not meant toi tell you how you must work, but to suggest how you **might** work.
Don’t have your own personal style? You’re welcome to try mine.Already have one? That’s cool, feel free to read on anyway!

## Credits
Heavely inspired by [Allars's UE Style Guide](https://github.com/Allar/ue5-style-guide.git)

# Index

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
    |  |  |--Programmers chance to mess here
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
# 2. Naming Convention

## 2.1. Base Asset Name
```Prefix_BaseAssetName_Variant_Suffix```\
```BaseAssetName``` should be simple and recognizible as well as the ```Variant``` if present.
For generic assets, use **digits** as ```Variant```.\
\
Examples:
- BP_Shovel_Broken;
- T_Umbrella_01_BC.

## 2.2. Asset Name Modifiers

Credits to [Starforge Games](https://github.com/StarforgeGames/UE-Style-Guide.git) for most of the suffixes and, more importantly, for reminding me of the many different types of assets.

### Sections

> - 2.2.1. [Animations](#animations)  
> - 2.2.2. [Artificial Intelligence](#artificial-intelligence)  
> - 2.2.3. [Blueprints](#blueprints)  
> - 2.2.4. [Materials](#materials)  
> - 2.2.5. [Texture](#texture)  
> - 2.2.6. [Miscellaneous](#miscellaneous)  
> - 2.2.7. [Paper 2D](#paper-2d)  
> - 2.2.8. [Physics](#physics)  
> - 2.2.9. [Sounds](#sounds)  
> - 2.2.10. [User Interface](#user-interface)  
> - 2.2.11. [Effects](#effects)  
> - 2.2.12. [Input](#input)  

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

### 2.2.11. Input

|Asset Type|Prefix|Suffix|Notes|
|--|--|--|--|
|Input Mapping Context|IMC|||
|Input Action|IA|||
|Force Feedback Attenuation|FFA|||
|Force Feedback Effect|FFE|||

# 3. Blueprint Coding Practices
