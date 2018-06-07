# androidlogcatviewer
exported from code.google.com/p/androidlogcatviewer

# How to build on Windows
```Bash
cd LogcatOfflineView
MKDIR classes
javac -d classes -sourcepath src -cp classes;lib\*;lib\x86_64\* src\com\logcat\offline\*.java
jar cfe AndroidLogcatViewer.jar com.logcat.offline.Main -C classes com -C src images
```
Unzip all libs in lib\*.jar, lib\x86_64\*.jar and zip all contents into AndroidLogcatViewer.jar
```Bash
jar ufe AndroidLogcatViewer.jar com.logcat.offline.Main
java -jar AndroidLogcatViewer.jar
RMDIR /Q /S classes
```

# Licenses
http://www.apache.org/licenses/LICENSE-2.0
