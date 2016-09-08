# System.Data.SQLite.Mac
Slightly modified version of System.Data.SQLite core project to target Xamarin.Mac.

Based off the source code for latest (version 1.0.102.0 as of this commit), downloaded at: https://system.data.sqlite.org/downloads/1.0.102.0/sqlite-netFx-source-1.0.102.0.zip

The project is configured with the following features:
* The compiler symbols are set to use only managed code (no interop assemblies)
* Uses Mono's native utf8 string marshalling support
* The csproj is set to target Xamarin.Mac .NET 4.5 Framework
* DllImport changed to use "libsqlite3_included.dylib" which must be included in the app bundle (can be found in the native sqlite nuget package)
