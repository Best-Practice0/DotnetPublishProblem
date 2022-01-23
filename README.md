# DotnetPublishProblem
A demonstration of a dotnet publish failure

run `dotnet publish -f net6.0` in the root and you will get the following error:

``
\DotnetPublishProblem\NotDirectReference\NotDirectReference.csproj : error MSB4057: The target "GetCopyToPublishDirectoryItems" does not exist in the project.
``

This solution consists of 3 projects. The main program, another project that the main program depends on, and a third project that was added as a Build Dependency (in Visual Studio right-click the project->Build Dependencies->Project Dependencies...).

The three projects all dual targeting Net6.0 and Net5.0.

Note that this is a problem when publishing the .sln.
