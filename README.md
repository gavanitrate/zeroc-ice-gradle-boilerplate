# zeroc-ice-gradle-boilerplate

## Requirements
1. Gradle 3.4.1
2. [ZeroC Ice 3.6.3](https://zeroc.com/distributions/ice)

## Usage
1. Place your .ice files in src/main/slice
2. Place your .java files in src/main/java
3. Run your desired command
    ```sh
    # watch .ice and .java files and rebuild on changes
    gradle watch -t

    # watch only .ice files and rebuild on changes
    gradle watch_slice -t

    # compile .ice files to .java files, just once
    gradle compileSlice
    ```
4. Make sure when executing any class files, that you include the ICE library in the classpath at compile time
    #### In IntelliJ IDEA, go to File > Project Structure > Modules and mimic these settings
    ![intellij settings](http://img04.imgland.net/gOscLk.png)
