#Introduction to Android Mobile Application Development

### How does a mobile OS work?

- A mobile OS typically starts up when a device powers on, displaying different application icons and UI elements to users.

<img src='https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/6y4pvD1DRZSuKbw9QzWUwA_b8d51a31cbb34c69b6b87ca94dcb0fe1_ADC1M1L2item3.png?expiry=1668556800000&hmac=AugJoiQ6oyuePlrr_yLOBudNqi8q9yxUWhBpXSqxAfQ'/>

### Android platforms:

- Chromebook
- Android TV
- Android Auto
- Wear OS 

### The Android OS architecture:

- Android software is built on top of open-source Linux kernel and many other C or C++ libraries exposed via application framework services.

- Among all the components, the Linux kernel perovides the main OS functions for smartphones and the Dalvik Virtual Machine (DVM) provides a platform for running an Android application. 
- An Android OS is a stack of software components roughly divided into five sections:
  + Applications
  + Applications Framework
  + Android Runtime
  + Platform libraries
  + Linux Kernel
- These are seperated into 4 layers:
  <img src='https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/qHi-z6qtQ3y4vs-qrQN8xQ_a0afdd3e0c364406851e2fefe72ce3e1_Picture-1.png?expiry=1668556800000&hmac=EMLEPO-Cgql1OfnBcfS_pMOzKinYl1sFaAsXHv1nu1Q' />

### Mobile CPU Architecture:

As of now, there are three main CPU architectures used in most smartphones - ARM, ARM64 and x86.
CPU types include:
- ARM: ARMv7 and armeabi
- ARM64: AArch64 and arm64
- x86: x86 and x86abi

Of these three, ARM is the most common as it is properly optimized for battery use.

ARM64 is an evolution of the original ARM architecture that supports 64-bit processing for more powerful computing and it's quickly becoming the standard in newer devices.

Then there's x86, which is a bit more powerful than the ARM CPUs, but not quite as battery-friendly, so it's the least commonly used for the three.

### Common libraries and packages:

- Image loading - Fresco
- Videos - ExoPlayer
- Networking - Retrofit

#### Quiz notes:

- **Quick boot** will remember the last state of your device so that when you run the Android emulator the next time it will show you the same screen.

- **Cold boot** will start your device as if you’re turning it on for the first time. 

### Project structure:

``.gradle``: configurations and files used for project building, they are automatically generated each time you try to compile a project.

``.idea``: used by Android Studio to store specific project metadata.

``gradle``: refers to Android's build system, which is a set of tools made available to developers to build, test, and run their applications; whenever you build or compile a project, build-related data is generated and held in this gradle or build folder.

``build.gradle``: specify and manage configuration options.

``gradlew``: file that is used by Gradle Android Studios build system; it is only created once and is updated whenever a new feature or plugin is required to build a project.

``local.properties``: this file contains information specific to your local configuration.

``settings.gradle``: this file handles the various settings for projects and modules

### Gradle:

<img src="/images/gradle.jpg" />

### Android manifest:

When you create a project:
- Android Studio generates a manifest (.xml)
- The manifest contains info about your app.
- This info helps you define permissions.