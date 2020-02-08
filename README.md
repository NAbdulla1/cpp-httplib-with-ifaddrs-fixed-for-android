This project is the combination of https://github.com/yhirose/cpp-httplib and https://github.com/morristech/android-ifaddrs to fix the `ifaddrs.h` error in Android SDK version 23 or lower.
<br/>
<br/>
<strong>Usage:</strong> clone this project in the root of cpp directory in android project and add the `add_subdirectory(cpp-httplib-with-ifaddrs-fixed-for-android)` in the root level CMakeLists.txt and link the `httplib`.
<br/>
<br/>
An example project is available here: https://github.com/NAbdulla1/Example-of-CPP-HTTPLIB
