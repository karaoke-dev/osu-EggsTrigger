# osu-Gameboy

[![NuGet](https://img.shields.io/nuget/v/osu.Framework.Eggs.GameBoy.svg)](https://www.nuget.org/packages/osu.Framework.Eggs.GameBoy)
[![NuGet](https://img.shields.io/nuget/dt/osu.Framework.Eggs.GameBoy.svg)](https://www.nuget.org/packages/osu.Framework.Eggs.GameBoy)

This is an unofficial Egg for osu!lazer

How to work : 
```Csharp
//Create gameboy
var gameboy = new GameBoyContainer();

//Load rom
string romPath = "Resources/ROM/Tetris.gb";
gameBoyContainer.LoadDevice(romPath, Path.ChangeExtension(romPath, ".sav"));

//Add to parent container
Add(gameBoyContainer);

//Run Gameboy device
gameBoyContainer.RunDevice();
```