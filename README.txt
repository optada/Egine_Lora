HI! My nick is - OPTada. This project - (GameEngine_Lora), is my pet-project. 
GitHub   : https://github.com/optada/Egine_Lora

my mail@ : druzhinin.optada@gmail.com

// --------------------------------------------------------------------------------------------------
// Description

This project is a simple version of a Engine_Dity (https://github.com/optada/Engine_Dity) - does not contain physics and sound. Built exclusively on my code and open standardized libraries. You can say that this is a "clean version" of my engine.

This version of the engine was used by me to defend my master's work. And quite successfully (5/5).

This project is a set of architectural and algorithmic solutions for rendering graphics, 
memory control, window control, input control.
The architecture of this project implements the idea of a game cycle.
The project handles most errors, and it also guarantees the correct release of resources 
created using its functionality.


// --------------------------------------------------------------------------------------------------
// Functional

project for WIN_x64

The project uses several independent subsystems, combining them in a common interface OPTada_Instance.

Each subsystem provides the necessary functions and implementations for solving specific problems:

1) Input -> Poll user input from the mouse and keyboard

2) Window ->  User window control under Windows, see ( https://github.com/optada/Class_Window )

3) Render -> This system implements classes for controlling DirectX11 rendering, 
providing classes for (controlling|loading|using) resources (shaders, grids, textures). 
As well as everything you need to control the rendering of DirectX11.
It contains the memory control subsystems 
and the DirectX11 resource manager (grids, textures, shaders, etc. ...)

Since the project is quick and educational, I will not describe the full functionality (see the code if necessary). 
Implemented obliquely render:
Light, the use of textures, shaders, grids, as well as automation of all this due to the rendering logic.
Hash optimization in the render pipeline to reduce video card access commands.
Transfer up to 100 light sources to a shader.
Using memory optimization by storing a copy of resources in the CPU memory to clean the GPU and load it again without accessing the HDD.
And a bunch of small optimization features for rendering objects.


// --------------------------------------------------------------------------------------------------
// Use

OPTada_Instance -> contains all primary actions for controll the program;

This engine is not a complete software product. You can take some parts of it and integrate it into your project, 
or use it as a basis, having altered it to your needs. 
(although I highly recommend using it only for educational purposes)


// --------------------------------------------------------------------------------------------------
// Usage tips

Most likely I will not do / remodel or support this project. Since it is more likely for challenge and training.

// --------------------------------------------------------------------------------------------------
If you find a mistake|bug|error, please describe it and write to me:
on my mail@ : druzhinin.optada@gmail.com
or GitHub   : https://github.com/optada/Egine_Lora
