```
dotnet build
cat ./files.foo
# Observe \t replaced by /t in resulting file.
# Caused by custom task in project file
```
