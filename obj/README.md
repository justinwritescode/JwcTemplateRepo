# JwcRepoSdk
This repository contains files that are common to all of my repositories. 
To restore the files, add a `.restoreproj` file to the root of your git repo with at least the following contents:

```xml
<Project Sdk="JwcRepoSdk" />
```

Alternatively, stick this line in any `*proj` file at the top level of your repo:

```xml
<Sdk Name="JwcRepoSdk" />
```

And add a `global.json` file with at least the following contents:

```json
{
    "msbuild-sdks": {
        "JwcRepoSdk": "the-latest-package-version"
    }
}
```

Then run the following command and voila! The files will be restored!

`dotnet restore *.restoreproj`


      
Built from [commit b98188b on branch main at 2023-01-11T00:49:47-05:00]
(https://github.com/justinwritescode/Common/tree/b98188b928a52088b5fc07b37c721b0bc8a6665d)
