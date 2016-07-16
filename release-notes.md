## Release notes for .NET Core 1.0.0 - VS 2015 Tooling Preview 2

You can read more about this release at https://blogs.msdn.microsoft.com/webdev/2016/06/27/announcing-asp-net-core-1-0/

This release contains the following.

### Web tooling updates for ASP.NET as well as Preview 2 tooling for Microsoft .NET Core 1.0.0

This release contains the latest tools to build great ASP.NET applications. It also contains Preview 2 tooling for Microsoft .NET Core 1.0.0.

### Template updates

 - **Default auth switched to No Auth**: In previous versions Individual Auth was the default authentication option. We have changed this to No Auth to simplify the default project contents.
 - **BundlerMinifier included**: In previous versions we were relying on gulp to bundle and minify client side content. We have changed this to use BundlerMinifier to simplify the default project contents and decrease the dependencies.

### FTP Publish support included

In this release we have added support to publish to FTP endpoints using the Visual Studio Publish Web dialog.

## Release notes for .NET Core 1.0.0 RC2 – VS 2015 Tooling Preview 1

You can read more about this release at https://blogs.msdn.microsoft.com/webdev/2016/05/16/announcing-asp-net-core-rc2

This release contains the following.

### RTM tooling for ASP.NET (ASP.NET, not including ASP.NET Core)

This release contains RTM quality support for ASP.NET. Including many bug fixes from previous releases.

### Preview 1 tooling for .NET Core and ASP.NET Core

This release contains Preview 1 tooling for .NET Core and ASP.NET Core. We have also fixed a number of issues from previous releases.

### Support for running EF Migrations on Publish

We have added support on the Web Publish dialog to execute Entity Framework Migrations during a publish using Web Deploy (aka MSDeploy).

### New Project updates

The templates provided in the File->New Project dialog have been updated. We now have three template entries in the New Project Dialog related to ASP.NET.

 - **ASP.NET Web Application (.NET Framework)**: This opens the One ASP.NET dialog with templates for ASP.NET. Including Web Forms, MVC, Web API, etc. These templates use `System.Web` and only run on Windows.
 - **ASP.NET Core Web Application (.NET Core)**: This opens the One ASP.NET dialog with templates for ASP.NET Core running on .NET Core. Since these are targetting .NET Core they can be used on all platforms (Windows, Linux and OS X). 
 - **ASP.NET Core Web Application (.NET Framework)**: This opens the One ASP.NET dialog with templates for ASP.NET Core running on .NET Framework. Since they are running on the .NET Framework, these templates will only run on Windows. You should use this if you have investments in libraries, or code, which are not compatible with .NET Core.

### Web linters

With this release we are including web linters including: ESLint, CSSLint, TSLint and CoffeeLint.

### Dependency updates

We have refreshed many of the packages used in the default templates provided by File -> New Project.

In addition we have updated to node version 5.4.1 and npm version 3.3.4.

### Updated support for xproj projects referencing csproj projects

We have updated the support for .xproj projects referencing .csproj projects. In the past we relied on a command line tool `dnu wrap`. We ran into many issues with that support and decided to re-implement it without using that command line tool.

### Links

For more info see https://blogs.msdn.microsoft.com/webdev/2016/05/16/announcing-asp-net-core-rc2/. If you have any problems using the release please file an issue at https://github.com/aspnet/tooling/issues.

For known issues see https://github.com/aspnet/Tooling/blob/master/known-issues.md.
