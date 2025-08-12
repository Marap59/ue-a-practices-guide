# ue-a-practices-guide
Practices for efficient naming conventions, organized content structure, and readable Blueprint code.
# Premise
This guide is not meant toi tell you how you must work, but to suggest how you **might** work.
Don’t have your own personal style? You’re welcome to try mine.Already have one? That’s cool, feel free to read on anyway!

## Credits
Heavely inspire by [Michael Allard's Style Guide](https://github.com/Allar/ue5-style-guide.git)

# Index

# Content Structure

## Prerequisites
As soon as the project is created, make a folder inside the Content folder and **name** it after the **project**. From now on, we will work in that specific folder.

*Optional*: Add a **Plugins** folder inside the Content folder, where you can move any folders added by plugins
## The Idea
The main idea is to make folder based on the type of **family** they are going to contain. With family I mean a group of assets that represents a category which may be: characters, weapons, vehicles.
In the case of assets used to build levels, we l
## Generic Example
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
# Naming Convention

# Blueprint Coding Practices
