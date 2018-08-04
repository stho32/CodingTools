# CodingTools
My standard coding tools, command line programs that I need on every computer

There are some tools that I need for a complete dev computer setup. 
I need them in my path and I need a few modifications on their configuration.

To make sure I can synchronize them on every computer I use, here comes "CodingTools".

CodingTools at this moment contains:
  - nuget v. 4.7.0
  - msbuild 2015 (=v14)
  
To set things up, clone the repo and set your path to contain the folder.
The easiest way should be: 
```powershell
	New-Item $Profile
	vim $Profile
```

Then enter e.g.:
```powershell
$ENV:PATH=”$ENV:PATH;c:\Projekte\CodingTools”
```

Run provided installers as needed.


## nuget

To set a fixed local directory for nuget packages, which will allow for more flexible 
combination of repositories of .net apps with sub repositories which also contain 
.net apps:

```powershell
	nuget config -set repositoryPath=C:\Nuget\packages
```
