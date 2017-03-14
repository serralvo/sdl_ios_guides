## Updating from 4.X.X to 4.3+

This guide is used to show the update process for a developer using a version before 4.3, using the `SDLProxy` to using the new `SDLManager` class available in 4.3 and newer. For our examples through this guide, we are going to be using the version 1.0.0 of the Hello SDL project. 

You can download this version [here](https://d83tozu1c8tt6.cloudfront.net/media/resources/hello_sdl_ios-1.0.0.zip). 

### Updating the Podfile
For this guide, we will be using the most recent version of SDL at this time: 4.5.5. To change the currently used version, you can open up the `Podfile` located in the root of the `hello_sdl_ios-1.0.0` directory. 

Change the following line

```
pod 'SmartDeviceLink-iOS', '~> 4.2.3'
```

to

```
pod 'SmartDeviceLink-iOS', '~> 4.5.5'
```

You may then be able to run `pod install` to install this version of SDL into the app. For more information on how to use Cocoapods, check out the [Getting Started > Installation](Getting Started/Installation) section.

After SDL has been updated, open up the `HelloSDL.xcworkspace`.

You will notice that the project will still compile, but with 10 deprecation warnings. 

![Deprecation Warnings](/assets/DeprecationWarnings.png)

!!! note
Currently, ``SDLProxy` is still supported in versions but is deprecated, however in the future this accessibility will be removed.
!!!


### SDLProxy to SDLManager


### Lock Screen Manager