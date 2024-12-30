# Thermal Engine Mod for Xperia 1 IV

**Description:**

Modified thermal config for balanced daily performance and unlocked endurance mode for the camera.  Due to overheating, to avoid lawsuits Sony throttled performance which is very noticable during camera usage. However there is an "Endurance Mode", that can push device to the limit, given that you have a special accessory to hold your device to avoid potential skin burning. This mod will allow you to record longer videos and get more FPS in games without a need to purchase any certified accessories. 


During your **normal usage** phone will heat less due to the lower CPU frequencies and screen wont forcefully switch to 60hz even if for some reason phone will reach the higher temperature. However some apps are force switch to 60hz, like YouTube. You can use SmartHertz app to force 120hz on those.

Frequencies for **Default** profile are following: **1574Mhz (Little)+1651Mhz (Big)+2054Mhz(Prime)+545Mhz(GPU). Max temperature is 58C**

**Camera** related profiles are the same as **Performance** profile.


**You can switch thermal profiles for individual apps with Game Enhancer:**

* **Performance** profile  will throttle way less aggressively, screen refresh rate will only drop if the display's temperature sensor will reach 45C. Frequencies are **1785.6Mhz+2496Mhz+2515.2Mhz+734Mhz. Max temperature is **61C****
* **Balanced** profile is the same as **Default** profile.
* **Battery mode preferred** has following frequencies **1267Mhz+1325Mhz+1728Mhz+492Mhz, Max temperature is 57C**



More info, changelog, tests and older versions are on [XDA](https://xdaforums.com/t/root-a13-thermal-engine-mod-ver-1-3.4585473/)

Config was uploaded to GitHub since version 1.3


**Instructions:**

  You will need Magisk or KernelSU:

1. Install this module [HuskyDG/magic_overlayfs](https://github.com/HuskyDG/magic_overlayfs)
2. After rebooting go to oem/etc with any root file manager, enable R/W and replace the thermal-engine.conf.
3. Make sure to set the same permissions and backup original files.
4. In the end you may want to go to /data/adb/modules/magisk_overlayfs and modify mode.sh to lock partition again (mode 2), this is done to avoid some apps detecting traces of modified system.
5. If you use KernelSU, you may want to add these lines to the end of file mentioned in the previous step:

<pre><code>
export OVERLAY_LEGACY_MOUNT=false
export DO_UNMOUNT_KSU=true
</code></pre>
