# MSBuild.Microsoft.VisualStudio.Web.targets

MSBuild targets for Web and WebApplications that come with Visual Studio. Useful for build servers that do not have Visual Studio installed.

Includes `.targets` files from Visual Studio 2013 Update 4 that can be found in the `C:\Program Files (x86)\MSBuild\Microsoft\VisualStudio\v12.0\{Web,WebApplications}` directories. 

The files are in the `tools\VSToolsPath` directory.

## Use

Install the NuGet package (or get it from [nuget.org](https://www.nuget.org/packages/MSBuild.Microsoft.VisualStudio.Web.targets/))

    PM> Install-Package MSBuild.Microsoft.VisualStudio.Web.targets

Include the `.targets` files in your `.csproj`

```xml
<Import Project="$(SolutionDir)\packages\MSBuild.Microsoft.VisualStudio.Web.targets.12.0.4\tools\VSToolsPath\WebApplications\Microsoft.WebApplication.targets" />
```

## Build

In command prompt

    nuget.exe pack

## License

Copyright (C) Microsoft Corporation. All rights reserved.
