```cd ~/install```

``` git clone https://github.com/flutter/flutter.git -b stable```

```flutter precache```

```flutter doctor```

Required 32-bit libraries for all modern 64-bit Ubuntu installs that want to run Android Studio:
```sudo apt-get install libc6:i386 libncurses5:i386 libstdc++6:i386 lib32z1 libbz2-1.0:i386```

Download Android Studio for Linux
https://developer.android.com/studio

Unpack the Android Studio 'tar.gz' file in to /opt not /usr/local

Launch android studio:
```cd /opt/android-studio/bin```
```./studio.sh```

Follow directions of installer

---
At some point if your system is fast enoguh it will guide you to "Configure VM acceleration on Linux"

```sudo apt-get install cpu-checker```

```egrep -c '(vmx|svm)' /proc/cpuinfo```

```kvm-ok```
expected output: "/dev/kvm exists KVM acceleration can be used"

Install KVM on Linux:
```sudo apt-get install qemu-kvm libvirt-daemon-system libvirt-clients bridge-utils```

---

Open Android Studio

Click "More Actions" at the bottom

In the menu that pops up click "SDK Manager"

Next to the default open tab of "SDK Platforms", click "SDK Tools"

Click "Android SDK Command-line Tools (latest)

Click "OK", and then "OK" again to start the download for this necessary tool that flutter doctor says we need

Accept license
```flutter doctor --android-licenses```

```sudo apt install cmake```

```sudo apt install ninja-build```

```sudo apt install libgtk-3-dev```

Run ```flutter doctor``` again to make sure all dependencies are met.

Update your path so you can run flutter commands in any terminal session. Just do it.
export PATH="$PATH:$HOME/install/flutter/bin"

Verify that the "flutter/bin" directory is in the PATH by running:
echo $PATH

Verify that the flutter command is available by running:
```which flutter``` and
```which flutter dart```
