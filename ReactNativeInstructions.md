# Spinning Up React Native App

## System Requirements

1. Current version of Android Studio installed is **Android Studio Hedgehog | 2023.1.1**.
2. System requirements for this version of Android Studio are
    * 64-bit Microsoft® Windows® 8/10/11
    * x86_64 CPU architecture; 2nd generation Intel Core or newer, or* AMD CPU with support for a Windows Hypervisor
    * 8 GB RAM or more
    * 8 GB of available disk space minimum (IDE + Android SDK + Android Emulator)
    * 1280 x 800 minimum screen resolution

3. System Specifications of PC it is being installed on
    * Windows Version: Windows 11 Pro 22H2
    * Processor: AMD Ryzen 7 PRO 6850U with Radeon Graphics        2.70 GHz
    * Installed RAM: 32.0 GB (30.8 GB usable)
    * Display Resolution: 2560 X 1600

## Installation Instructions

Necessary tools to download and run android studio are :

1. Node
2. JDK
3. React Native

### Node

The installer of Node can be downloaded from [Node's Official Website](https://nodejs.org/en/download). Download the LTS version. Alternatively, you can use package manager to do the same. Use winget, if you are using Windows operating system. The command do that is ```winget install OpenJS.NodeJS.LTS```  

```npm``` package manager will also be installed with Node.

### JDK

There are many different versions of JDK from different vendors like Microsoft, Oracle, etc. The version installed for this setup is from [Adopt](https://adoptium.net/).

### React Native

The installation for React Native is pretty straightforward. Use ```npm``` to install it using ```npm install -g react-native-cli```.

### Android Studio

The installation for the Android Setup as simple as following setup wizard.

## Configuration Steps

1. Once, Android Studio is installed, go to settings tab and under SDK Manager go to SDK Platform section and select the latest SDK and apply the settings. Android Studio will automatically download and install it.
2. After it is installed, go to SDK tools section and make sure that android SDK platform tools is selected.
3. The React Native tools require some environment variables to be set up in order to build apps with native code.
    1. Open the Windows Control Panel.
    2. Click on User Accounts, then click User Accounts again
    3. Click on Change my environment variables
    4. Click on New... to create a new ANDROID_HOME user variable that points to the path to your Android SDK:
4. Add platform-tools to Path
    1. Open the Windows Control Panel.
    2. Click on User Accounts, then click User Accounts again
    3. Click on Change my environment variables
    4. Select the Path variable.
    5. Click Edit.
    6. Click New and add the path to platform-tools to the list.

## Project Creation

1. To create the react native project, use the ```npx``` executable in the directory you want to initialize the project. The command to do so us ```npx react-native init AppName```. By default the project will be TypeScript based to change that suffix the mentioned command with ```--version 0.70.0```.

## Running the Project

1. To run the project you need to add the virtual device first which can be added using the device manager(on side bar).
2. Mention the specifications of device you want and wait for it to get added.
3. To run the device, go the Running Devices section and add the device you just created and it should start to boot.
4. Once it is booted, run ```npx react-native doctor``` to make sure that all the dependencies are installed and recognized.
5. Then enter ```npm start``` to start the app.

## Troubleshooting

Common errors when setting up the development environment or running the project include  

1. Android SDK not found  
    To solve it:  
    Go to your project then go to the android directory and create a file with the following name – local.properties
    Open the file and paste your Android SDK path like below:  
    ```dir=C:\\users\\{username}\AppData\\Local\\Android\\sdk```  
    After that change your directory to android and run ```gradlew clean```.
2. Java home path
    Make sure your Java home path is set to the correct location.

## Resources

1. <https://www.linkedin.com/pulse/which-java-jdk-should-you-use-incus-data-pty-ltd>
2. <https://reactnative.dev/docs/environment-setup>
3. <https://www.geeksforgeeks.org/how-to-fix-sdk-location-not-found-in-android-studio/>
