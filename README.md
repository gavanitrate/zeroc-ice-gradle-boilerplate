# zeroc-ice-gradle-boilerplate

## Requirements
1. Gradle 3.4.1
1. [ZeroC Ice 3.6.3](https://zeroc.com/distributions/ice)

## Usage
1. Enter the path to your ICE install in `build.gradle:18`
1. Place your .ice files in `src/main/slice`
1. Place your .java files in `src/main/java`
1. Run your desired command
    ```sh
    # watch .ice and .java files and rebuild on changes
    gradle watch -t

    # watch only .ice files and rebuild on changes
    gradle watch_slice -t

    # compile .ice files to .java files, just once
    gradle compileSlice
    ```
1. Make sure when executing any class files, that you include the ICE library in the classpath at compile time
    #### In IntelliJ IDEA, go to File > Project Structure > Modules (image below) and make sure the ICE library is included at compile time, in any/all of the modules you want
    ![intellij settings](https://user-images.githubusercontent.com/8264198/37464581-7909d9c4-28a4-11e8-8b00-d0ca4a203070.png)
