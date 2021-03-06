<p align="center">
<a href="#"><img src="http://i.imgur.com/ohEL0KO.png"/></a>

<a href="http://www.ferris.edu/dagd/"><img src="https://img.shields.io/badge/made%20by-Ferris%20State%20University-blue.svg?style=flat-square"/></a>
<a href="https://unity3d.com/"><img src="https://img.shields.io/badge/engine-Unity-brightgreen.svg?style=flat-square"/></a>
<a href="https://docs.unity3d.com/Manual/webgl-gettingstarted.html"><img src="https://img.shields.io/badge/platform-WebGL-brightgreen.svg?style=flat-square"/></a>
<a href="https://github.com/AndrewK9/Resort-Visualizer/issues"><img src="https://img.shields.io/badge/issues-0%20open-brightgreen.svg?style=flat-square"/></a>
<a href="https://github.com/AndrewK9/Resort-Visualizer/blob/master/LICENSE"><img src="https://img.shields.io/badge/license-NonCommercial%20CC%204-brightgreen.svg?style=flat-square"/></a>
</p>

## Table of Contents
1. [Introduction](#introduction)
1. [Install](#install)
1. [Usage](#usage)
1. [Team](#team)
	- [Product Owner](#product-owner)
	- [Programmers](#programmers)
	- [Artists](#artists)
1. [Screenshots](#screenshots)
1. [Naming Conventions](#naming-conventions)
	- [3D Files](#3d-files)
	- [Textures](#textures)
1. [Programming Style](#programming-style)
	- [Visual Appeal](#visual-appeal)
	- [Variable Prefixes](#variable-prefixes)
	- [Using Properties](#using-properties)
1. [Contribute](#contribute)
1. [License](#license)

## Introduction
This Resort Visualizer prototype is being created for [Pillar Workshop](http://www.pillarworkshop.com/) by students at [Ferris State University](http://www.ferris.edu/dagd/). The goal of this project is to provide the client with a 3D web-based interactive visualizer. The visualizer will run on the WebGL JavaScirpt API and will be built in Unity 3D.

## Install
This project uses [Unity](https://unity3d.com/) and [WebGL](https://docs.unity3d.com/Manual/webgl-gettingstarted.html). Go check them out if you don't have them locally installed.

## Usage
Currently, this section is barren, as new features are built into the project this section will be updated.

## Team
#### Product Onwer

Logan Armstrong |
|-----|
| [Email](larmstrong30298@gmail.com) |

#### Programmers

Kyle Andrews |
|-----|
| [Email](andrewskyle28@gmail.com) |

#### Artists

Brent Perko | Ed Chrzanowski | Cameron Ames | Brad Vriesman | Jole Striegle |
|-----|-----|-----|-----|-----|
| [Email](brentp3rk0@gmail.com) | [Email](chrzane1@ferris.edu) | [Email](amesc3@ferris.edu) | [Email](vriesmb@ferris.edu) | [Email](striegj@ferris.edu) |

## Screenshots
Currently, this section is barren, as new features are built into the project this section will be updated.

## Naming Conventions
#### 3D Files
```
Working Files:
(yyyy-mm-dd)_(ObjectName)_(Unwrapped (U) or NoUnwrap (NU))_(iteration #)_(initials of person who saved iteration).(obj or fbx)

Example:
2017-01-29_EiffelTower_NU_05_EC.obj
```

#### Textures
```
Working files:
(yyyy-mm-dd)_(ObjectName)_(initials of person who saved iteration).(texturing software)

Example :
2017-01-29_EifelTower_EC_.psd

Finals:
(Final)_(ObjectName)_(initials of person who saved iteration)_(mapname:DIFF,SPEC,NORM,etc.).png

Example:
Final_EifelTower_EC_DIFF.png
```


## Programming Style
#### Visual Appeal
We will be following the standard naming conventions set by [Microsoft's .NET Framework](https://msdn.microsoft.com/en-us/library/ms229042(v=vs.110).aspx), see Programming Style below for specific changes.

Tabs over spaces, for this project we will be using four column tabs and the Allman indent style. All selection and iteration single-line statements will have a beginning and ending brace.
```
if(x == y) { return true; }
```

#### Variable Prefixes
All private variables will have an underscore prefix.

#### Using Properties
All global variables must declare their using properties and private variable counterparts.
```
private int m_numOfCows = 2;
public int g_numOfCows
{
    get
    {
        return m_numOfCows;
    }
}
```
We should never allow other scripts to set a public global variable, instead we’ll create a public function that sets the private variable.
```
public void SetNumOfCows(int newNumOfCows)
{
    m_numOfCows = newNumOfCows;
}
```


## Contribute
Feel free to [open an issue](https://github.com/AndrewK9/Resort-Visualizer/issues) or clone this project to start working on your own, however, fixes and features contributions will only be accepted from Ferris State University students who are currently on the Resort Visualizer team.

## License
[Creative Commons Attribution-NonCommercial 4.0 International Public License](https://github.com/AndrewK9/Resort-Visualizer/blob/master/LICENSE) (c) [Ferris State University](http://www.ferris.edu/dagd/)
