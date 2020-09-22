# Unity Intellisense for Code on Manjaro Linux
This guide assumes you already have Unity and Visual Studio Code or Code OSS(Recommended) Installed.
## Install Dependencies
Install the .NET core SDK, Mono and MS Build.
```shell
sudo pacman -Syu dotnet-sdk mono mono-msbuild
```
Install the Unity Debugger Extension for Code.
Open Code and press "CTRL+P", paste the following and hit enter.
```
ext install Unity.unity-debug
```
## Configuration
### Unity External Editor
In Unity Change the External Script Editor By Going
Edit > Preferences > External Tools > External Script Editor
#### Native
In the drop down menu select either code option "/bin/code" or "/usr/bin/code"
#### Snap
In the drop down menu select Browse and go to "/var/lib/snapd/snap/bin/code"
### Configuring The C# Extension
Go to File > Preferences > Settings
In the side menu click on the extension drop down then the C# configuration and set "Omnisharp: Use Global Mono" to Always.
