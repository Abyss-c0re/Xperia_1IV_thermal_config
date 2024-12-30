# Thermal Engine Mod for Xperia 1 IV

If you want stable 120hz with a better battery life and lower heat during normal usage with forced endurance mode for camera (longer 4k120FPS recording) and game enhancer's performance profile, look no further!

**Description:**

Config was uploaded to GitHub since version 1.3

More info, changelog, tests and older versions are on [XDA](https://xdaforums.com/t/root-a13-thermal-engine-mod-ver-1-3.4585473/)

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


  


