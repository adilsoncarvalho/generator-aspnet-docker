generator-aspnet-docker
=======================

This is a simple container to make it quick to use [OmniSharp/generator-aspnet][0] in order to generate several projects from the [dotnet/templating][1].

## How to use

    docker run --rm \
      -v "$(pwd):/var/stage" \
      generator-aspnet-docker \
      [project-type] [project-name] [ui-framework]

> Important: don't forget to mount your project directory onto `/var/stage`

## Project Types

The valid project types are:

- `web` for Empty Web Application
- `console` for Console Application
- `mvc` for Web Application
- `mvcbasic` for Web Application Basic
- `webapi` for Web API Application
- `nancy` for Nancy ASP.NET Application
- `classlib` for Class Library
- `mstest` MSTest Test project (MSTest)
- `xunit` xUnit Test project (xUnit.net)
- `fsharp_web` for F# Empty Web Application
- `fsharp_console` for F# Console Application
- `fsharp_classlib` for F# Class Library
- `fsharp_webapi` for F# Web API Application
- `fsharp_mvcbasic` for F# Web Application Basic
- `fsharp_mstest` for F# Unit Test project (MSTest)
- `fsharp_xunit` for F# xUnit Test project (xUnit.net)

## UI Frameworks

The valid UI framework types are:

- `bootstrap` for Bootstrap (this is the default and does not have to be specified explicitly)
- `semantic` for Semantic UI

> NOTE: This is a copy of the [original documentation][2] and it would be wise to check them for an updated value.


[0]: https://github.com/OmniSharp/generator-aspnet
[1]: https://github.com/dotnet/templating
[2]: https://github.com/OmniSharp/generator-aspnet#command-line-automation
