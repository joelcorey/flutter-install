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


