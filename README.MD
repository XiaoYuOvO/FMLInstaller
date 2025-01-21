## For Developers
### Configure this project
1. Install the Exe4j bundler and a Java8 Jdk
2. Modify the jdk path and the exe4j path in `fmlinstaller.properties` to the correct paths on your machine
3. Modify the path in the line `3,4,47` of both file `FML_Installerx32.exe4j` and `FML_Installerx64.exe4j` to the project location on your machine
4. Load the Ant build script `fmlinstaller.xml`
5. Add a dependency of `gson-2.2.2` to your classpath

### Make a FishModLoader Installer release
1. Replace the `FishModLoader.jar` under the `src/net/xiaoyu233/fmlinstaller` to your released one
2. Change the version number in `version.properties` under src folder
3. Change the version number in both `FML_Installerx32.exe4j` and `FML_Installerx64.exe4j` in line 9(Open them as plain text)
4. Open the Ant Build panel and run the `Build_32-64` target(Disable the filter if you can't see it)
5. After build finished you can find your installer in the project dir