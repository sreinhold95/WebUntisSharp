# <img src="https://raw.githubusercontent.com/mrousavy/WebUntisSharp/master/Images/Logo.png" width="50"> WebUntisSharp
A Wrapper of the [WebUntis](http://www.untis.at/Downloads/int/Manuals/de/WebUntis.pdf) JSON API for .NET

<img src="http://sankt-ansgar-schule.de/wp-content/uploads/2016/08/WebUntis.png">

# How to use

### 1. Add Binaries
   + NuGet
      * [WebUntisSharp is also available on NuGet!](https://www.nuget.org/packages/WebUntisSharp)   Install by typing `Install-Package WebUntisSharp` in NuGet Package Manager Console. (Or search for `WebUntisSharp` on NuGet)

   + Manually
      1. [Download the latest Library (.dll)](https://github.com/mrousavy/WebUntisSharp/releases/download/1.0.0.2/WebUntisSharp.dll)
      2. Add the .dll to your Project   (Right click `References` in the Project Tree View, click `Add References` and `Browse` to the `.dll` File)

### 2. Create WebUntis Object
* C#:
```C#
WebUntis untis = new WebUntis("mrousavy", "password1234", schoolUrl, "WebUntisSharp API");
```

* VB:
```VB
Dim untis As WebUntis = new WebUntis("mrousavy", "password1234", schoolUrl, "WebUntisSharp API");
```

### 3. Send Requests
* C#:
```C#
var timegrid = await _untis.GetTimegrid();
```

* VB:
```VB
Dim timegrid As Timegrid = await _untis.GetTimegrid();
```
