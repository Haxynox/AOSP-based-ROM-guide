#Where is my tea#

## Introduction ##


So as long as you know how to cherry-pick and get around most of the errors, you're good to go.

In this guide, we'll cover what you'll need to cherry-pick (and that too where) and how to make some tea

## Making the tea ##

```bash

Just joking lol

```

But since not everybody likes tea,

[![Move on mate](http://img.youtube.com/vi/3STk-HcfHjQ/0.jpg)](http://www.youtube.com/watch?v=3STk-HcfHjQ)

_that's a youtube link_

## Moving on ##

Now to focus on the commits that you need to pick in order to get the ROM booting, you'll have to pick the following commits:

NOTE: Order matters.
NOTE2: I'm going to assume that the terminal has been directed to the root of the ROM source

### "Frameworks/" stuff ###

1. **frameworks/base**

```bash
cd frameworks/base
git fetch https://github.com/Haxynox/android_frameworks_base aosp-6.0

git cherry-pick 0c9ff4407aa3e141d79cb663125ef0daa9751121
git cherry-pick 44290a814f22d64a43c3c1ebbdbe95b93d3bdf8a
git cherry-pick 23727c6a304ce72faebc9bf4cd5b5ca229983f0a
git cherry-pick 4fb87be6a1e3dae1ba84c6c961bab4e56093960e
```

[base](https://github.com/Haxynox/android_frameworks_base)

2. **frameworks/av**
```bash
cd frameworks/av
git fetch https://github.com/Haxynox/android_frameworks_av aosp-6.0

git cherry-pick 1750a0844515d02146a33caad9c32a8f42fafb36 
git cherry-pick 0c9c5ad6ef18252264bb55cfec3405cf3eec49c8
git cherry-pick 43648ea5b54887f786f566bc8d19070cc15dbb4b
git cherry-pick 90232427855fda8d2d656d41a52d43a36b205d35
git cherry-pick ec6b69268b2a330e386ad195f35e56e85b032cac
```

[av](https://github.com/Haxynox/android_frameworks_av)

3. **frameworks/native**
```bash 
cd frameworks/native
git fetch https://github.com/Haxynox/android_frameworks_native aosp-6.0

git cherry-pick ca40112135d23de3bc303b8fa33145c33f3445c8
git cherry-pick da03e2f81c45a81783f9caf7beb1c23b020c335d
git cherry-pick f9202ff6d6750f89aef433d7320558da14ee8b69
git cherry-pick 45a014ce5de5dd90b4016039528a11e61f902bf6
git cherry-pick e8ec5bc8d9189ae7f07960cc5437bc1c01a5bc6d
git cherry-pick 1f721a502fe76b96f7bbe62e64c3bf70ef74b720
git cherry-pick 0944e8d97200852710c1696bc11796814e52bbcc
git cherry-pick 42bd11ddee4c80de29d9d2971498922c96f9934e
git cherry-pick fbb384dc5d997b3c87fed3e6e735ebfd7a0d1dbf
git cherry-pick d00f0ea27d5976c5a3bc6260efe3ef1938303c48
git cherry-pick b33d1e7084022a4b71c8f05834114e6489abf2c1
git cherry-pick b17d19cceaf9cc64ab06be680b102dfe8a399611
```

[native](https://github.com/Haxynox/android_frameworks_native)

4. **frameworks/opt/telephony**
```bash
cd frameworks/opt/telephony
git fetch https://github.com/Haxynox/android_frameworks_opt_telephony aosp-6.0

git cherry-pick e00cb429a8b423a162d9ea432a7fa2da7c360968
git cherry-pick f9112171a6161d563e7545c6566dff37a3363cc9
git cherry-pick 6733e381dd4404dac1394468291eaf45ee2dd8ad
git cherry-pick dc17eda6ec2f8e1ed9772eccd8c3bee2d18df79c
git cherry-pick e1b257784e1ac6b28af1b9cbecb8ae81cfe1e9bf
```

[opt/telephony](https://github.com/Haxynox/android_frameworks_opt_telephony)

5. **frameworks/opt/net/wifi**
```bash 
cd frameworks/opt/net/wifi
git fetch https://github.com/Haxynox/android_frameworks_opt_net_wifi aosp-6.0

git cherry-pick 815a3d921f4fdf19530a64ec2b2ca8f276f2adab
git cherry-pick b388cc29559874bf0cdced31dcaf013df314e867
```

[opt/net/wifi](https://github.com/Haxynox/android_frameworks_opt_net_wifi)

### "Hardware/" stuff ###

1. **hardware/ril**
```bash
cd hardware/ril
git fetch https://github.com/Haxynox/android_hardware_ril aosp-6.0

git cherry-pick df8dee1bc2431cef623250ffe7da8da7853feb45
git cherry-pick 85cc3aae62d7164802d0c6c441d116cfad88a88e
```

[ril](https://github.com/Haxynox/android_hardware_ril)

2. **hardware/broadcom/wlan**
```bash
cd hardware/broadcom/wlan
git fetch https://github.com/Haxynox/android_hardware_broadcom_wlan aosp-6.0

git cherry-pick de7ba335593cd66efb5e6beddac07fb0696c0fe9
```

[broadcom/wlan](https://github.com/Haxynox/android_hardware_broadcom_wlan)

3. **hardware/broadcom/libbt**
```bash
git fetch https://github.com/Haxynox/android_hardware_broadcom_libbt aosp-6.0

git cherry-pick 66d2b35a79d28963863c598920c5138668778de0
git cherry-pick af1b1428e6576413b3fab4019b1376103ebfe7cc
git cherry-pick 40ecea359289428378adb76e920063e96275b0a3
git cherry-pick 963b3f45fe5f7b87f09455f8c7722458ef77c611
git cherry-pick 0582994069f11dc695028606af8e97c1e4c32a42
git cherry-pick 42e09d5977a5fbe66d0882004d3f457d62f47d4e
git cherry-pick 03b9c743439e48a6e45e8333d3b1b667792f360e
git cherry-pick 040c049544d6a13978f4111ded8f52afa840f185
git cherry-pick 8f819dd32727b427ea6d8da95490cae48a78abeb
git cherry-pick 0354a388350644308eedc3438b41ea6f51af18c7
```

[broadcom](https://github.com/Haxynox/android_hardware_broadcom_libbt)

4. **hardware/libhardware_legacy**
```bash
cd hardware/libhardware_legacy
git fetch https://github.com/Haxynox/android_hardware_libhardware_legacy aosp-6.0

git cherry-pick 8dd24849a0a4be60a6eef45fce7f61a087921637
git cherry-pick 11281e8dc08d918cdab3b39209adf6f3d5686075
git cherry-pick 5f89fb14c11f46f32984c371654406279fdb48bf
git cherry-pick 28a233710da213fbc7400b7b2894dc0a0300f989
git cherry-pick ca0658e7471d3767bfb0b1c3da7c54640e5bf055
git cherry-pick 231dfefc44854fad25b9b7d116c24d78c490c4ab
```

[libhardware_legacy](https://github.com/Haxynox/android_hardware_libhardware_legacy)

5. **hardware/libhardware**
```bash
cd hardware/libhardware
git fetch https://github.com/Haxynox/android_hardware_libhardware aosp-6.0

git cherry-pick ab398d72e22bd8ff8baf448da345dc2c5926b993
git cherry-pick f3cf3dd5e49b2cd7ba5e3fb941c7d4f09f9ad5e8
git cherry-pick bc33b8b0c9a1e19a388db734f40e469b56880d3e
```

[libhardware](https://github.com/Haxynox/android_hardware_libhardware)

### Important stuff ###

external/stlport because you need your ril running :)
```bash
git clone https://github.com/Haxynox/android_external_stlport external/stlport aosp-6.0
```

You may face some weird errors if you are on a ROM that is purely meant for Nexus only and they might lack some necessary commits. If that is the case, you should go checkout our
[system/core](https://github.com/Haxynox/android_system_core "Where")
[system/extras](https://github.com/Haxynox/android_system_extras "Is")
[system/vold](https://github.com/Haxynox/android_system_vold "Goddamn")
[haxynox_build](https://github.com/Haxynox/haxynox_build "TEA")
repos

If you face an error and have fixed it, you can "git commit -a" to save the commit :)

Also, if you plan on releasing source, and you don't have proper authorship on the commit for some reason, you can commit as such:
```bash
git commit --author="Gokul Balram <gokulbalram@gmail.com>"
```
With my name and email replaced with that of the original author of course.

I think that should be it.
