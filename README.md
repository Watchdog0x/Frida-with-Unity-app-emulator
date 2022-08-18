# Setup emulator

1 ) Download andriod https://developer.android.com/studio

<img src="https://user-images.githubusercontent.com/84445039/185476724-ad53ef1d-7435-49c2-a8bf-c07a038fa7e7.PNG" width="50%" height="50%"/>
<img src="https://user-images.githubusercontent.com/84445039/185476789-8081de76-2ffb-4763-b456-18a0f3677685.PNG" width="50%" height="50%"/>
<img src="https://user-images.githubusercontent.com/84445039/185476818-99d724e3-704a-4d3a-9279-2654ad1f5403.jpg" width="50%" height="50%"/>

Now run it. When it booted go to step 2 

## Install Magisk on emulator
2 ) Download rootAVD 
https://github.com/newbit1/rootAVD/archive/refs/heads/master.zip


<img src="https://github.com/newbit1/video-files/blob/master/rootAVD_Windows.gif" width="50%" height="50%"/>

```bash 
.\rootAVD.bat ListAllAVDs
```

```bash 
.\rootAVD.bat %LOCALAPPDATA%\Android\Sdk\system-images\android-30\google_apis_playstore\x86\ramdisk.img
```

## Install MagiskFrida
3 ) Download magisk-frida https://github.com/ViRb3/magisk-frida/releases \
on emulator and install it with Magisk Modules  \
\
And it will look like this when it done


<img src="https://user-images.githubusercontent.com/84445039/185479184-aa9746e0-346c-4913-8b5a-79a0683d7571.PNG" width="50%" height="50%"/>

 

## Frida NativeBridge


```bash 
frida -Uf learn.frida.unity --realm=emulated --no-pause
```


### Now you can find the libil2cpp.so addresses 

You can test it with 
```bash
Module.findBaseAddress("libil2cpp.so")
```

<img src="https://user-images.githubusercontent.com/84445039/185480281-6b00a8ab-f7d3-47b1-a9a1-aa4d9cb2c286.PNG" width="50%" height="50%"/>

