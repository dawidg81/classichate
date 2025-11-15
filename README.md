ClassicHate is a Classic Minecraft-like custom client compatible with CSP and CPE. The code is from ClassiCube and will be changed and customized in the future.

Idea by Ludinko23

Cross-Compiling on Linux!

How to build for Linux:
```
make linux
```
Dependencies
```
sudo apt install build-essential libx11-dev libxi-dev libgl1-mesa-dev libopenal-dev libcurl4-openssl-dev
```

How to build for Windows:
```
make mingw CC=i686-w64-mingw32-gcc CXX=i686-w64-mingw32-g++
```
You will need MinGw32
```
sudo apt install gcc-mingw-w64-i686 g++-mingw-w64-i686
```

How to build for Windows 64 bit
```
make mingw CC=x86_64-w64-mingw32-gcc CXX=x86_64-w64-mingw32-g++
```
You will need MinGw64
```
sudo apt install gcc-mingw-w64-x86-64 g++-mingw-w64-x86-64
```
How to build an APK installation file for Android:
```
cd android
./gradlew
```
Dependencies
```
sudo apt install git cmake ninja-build openjdk-11-jdk build-essential
```
Android NDK
```
mkdir -p ~/Android
cd ~/Android
wget https://dl.google.com/android/repository/android-ndk-r25b-linux.zip
unzip android-ndk-r25b-linux.zip
```
Android SDK
```
cd ~/Android
wget https://dl.google.com/android/repository/commandlinetools-linux-9477386_latest.zip
mkdir -p sdk/cmdline-tools
unzip commandlinetools-linux-9477386_latest.zip -d sdk/cmdline-tools/latest
```
To set enviroment variables
```
export ANDROID_NDK_HOME=~/Android/ndk/android-ndk-r23
export PATH=$ANDROID_NDK_HOME:$PATH
```
*may not be 100% accurate sorry guys.*


