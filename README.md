# bin
Binaries and Installers for public consumption.

This project is a collection of resources to help Windows users get started with Lua. The imputis has been my own frustration finding a straight line in using Lua with Windows 10.

## Getting Started

If you just want to try Lua on Windows 10+, download the 32 Bit version of the Lua 5.3 installer. This will install the latest Lua, plus a de-facto standard component that allows access to the filesystem. Lua can now be used from the command line (any current cmd or powershell windows will need to be re-opened) or by opening your start menu and typing "Lua" and clicking on the icon. 

**No other components are available at this point. You will have to download and install LuaRocks yourself. Any Rocks that require C/C++ will require either mingw or Visual Studio (Professional?) to be installed on the computer.** *I am working towards fixing this situation.

## What about auto-complete for Lua and fancy debugging?

If you are looking for an excellent Integrated Development Environment (IDE) akin to Visual Studio for Lua - repleat with tons of samples and tutorials - then please download and support https://studio.zerobrane.com. This project and ZeroBrane are not configured to work togther out of the box, but ZeroBrane is configurable. See https://studio.zerobrane.com/doc-general-preferences (Interpreter Path). Either way, it probably won't make a difference to you. ZeroBrane comes installed with a wide range of "Lua flavours". 

The WinLua project is not a replacement for ZeroBrane. WinLua is about bog-standard Lua as God intended it [1].

## Background

There are many excellent resources for Lua on Windows but some of them are out of date, and others are too complex for the average user. The combination of these hurdles make learning Lua on Windows and knowning what is current very difficult. *I wanted a simple installer that would install and remove Lua so I could hack at it.* I've tried to introduce some of my friends to Lua that are *very* technical but are not software developers. It took them months of poking around until they found something that the *think might* work, but... My experience has been similar. 

## What is wrong with the current solutions?

One of my goals is to outline all the Windows resources and their state of support in the Wiki. I shall elaborate there. 

That said, LuaBinaries is an excellent, current distribution of Lua based on MinGW (Minimum GNU for Windows). It's an excellent distribution but does not provide an installer and to the best of my knowledge requires additional MinGW resources. The binaries do not include a *.lib files that is required to link when using Visual Studio (namely LINK.exe). It's still *not quite* the Windows way...
 
 
 [1] I jest, I mean the latest release of Lua from PUC-Rio. http://www.puc-rio.br/index.html
