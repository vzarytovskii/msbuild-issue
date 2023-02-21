```
dotnet build
cat ./files.foo
```
Observe \t replaced by /t in resulting file when running on Linux, runs fine on Windows.

Caused by custom task in project file, it pretty much joins all files by glob into one, and at some point thinks that text is a path(?) and replaces separators to the "correct ones" for the platform (Linux)
