# keytocomment-gradle

The simple [Beatunes](https://www.beatunes.com) "keytocomment" 
[example plugin](https://github.com/beatunes/plugin-samples), built using [Gradle](https://gradle.org).
 
Interested in Beatunes plugins, but prefer using Gradle over [Maven](https://maven.apache.org)? Me too. The source code 
in this project is unchanged, but with these changes:

* A `build.gradle` file instead of a `pom.xml`
* The `plugin.xml` version template string has been changed from `${pom.version}` to just `${version}` (this is 
replaced by the version declared in the build files when the jar file is created).

## Building

Windows:
```Batchfile
gradlew.bat build
```

Linux:
```Shell
./gradlew build
```

You can find the built JAR file as `build/libs/keytocomment-gradle-<version>.jar`.

## Installing

Copy that jar file into your `plugins` directory. On my Windows 10 installation, it's in the user's 
`AppData\Local\tagtraum industries\beaTunes\plugins` directory, rather than where Beatunes itself is installed.

## License

[LGPL 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html).