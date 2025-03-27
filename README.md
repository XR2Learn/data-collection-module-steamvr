# Data Collection Module

## Compatibility

The Data Collection Module requires and is compatible with the SteamVR framework.
If used, the Shimmer module requires a Windows 10 or 11 operating system.

## Pre-Installation Steps

### Google Protobuf
Follow the guide at https://github.com/GameWorkstore/google-protobuf-unity

### System.IO.Ports

#### Solution 1

Go to: `Edit → Project Settings → Player → Other Settings → Configuration`<br>
Change __Api Compatibility Level__ from `.NET Standard 2.1` to `.NET Framework`.
- For Unity 2021 or newer: `.NET Framework`
- Older Unity versions: `.NET 4.x`

#### Solution 2

If you prefer to stay on .NET Standard 2.1, you can manually import `System.IO.Ports.dll` into Unity:
 - Locate the DLL: `C:\Windows\Microsoft.NET\Framework\<version>\System.IO.Ports.dll`
 - Alternatively, you can get it from the official Microsoft packages or NuGet (https://www.nuget.org/packages/system.io.ports/).

1) Create a folder in your Unity project (e.g., Assets/Plugins).
2) Drag and drop the DLL into this folder.
3) Select the DLL in Unity’s Project window
   - In the Inspector, set the Platform settings.
4) Unity will recompile your scripts, and `System.IO.Ports` should now be accessible.

## Usage

TBD
