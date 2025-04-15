# Comulator
> [!IMPORTANT]
> This library is brand new and still in active development; consider this an open beta version.

Comulator is a .NET standard 2.1 library that provides cross-platform, drop-in replacements for otherwise Windows-only COM objects.

This package is originally made for interpreters transpiling legacy code (like ASP Classic, VBScript and VBA) over to .NET to run via Roslyn on non-Windows hosts. 

As these legacy languages tend to rely on COM objects for basic operations (like writing to and reading from a hashmap/dictionary, operating on the filesystem, sending HTTP requests, handling XML or JSON and more), this package provides drop-in replacements for commonly used COM objects. These replacements target .NET Standard 2.1 and can run on all .NET runtimes that support it.

The COM replacements are provided as a standalone package (This package) for anyone that has a use for them.

## COM Replacement availability
> [!Important]
> Support for many common objects is currently missing, as the package is in active development.

Comulator offers drop-in replacements for the following COM objects out of the box:

## Extendability
While Comulator provides replacements for the most commonly used COM objects out of the box, it's impossible to offer replacements for all COM objects out there. As such, the library has been set up to easily be extendable with custom COM reimplementations. You can register these directly with Comulator, or make a nuget package that registers itself as a Comulator plugin (docs to follow). It would also be hugely appreciated if you're willing to contribute these COM replacements back to Comulator for others to use.
