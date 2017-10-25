Ninja-OS OREO
===========
**From The Shadow**

Credits
-------
* [**GZOSP (Base)**](https://github.com/AOSP-JF-MM)
* [**JDCTEAM**](https://github.com/AOSP-JF-MM)
* [**LineageOS/Cyanogenmod**](https://github.com/LineageOS)
* [**Pure Nexus**](https://github.com/PureNexusProject)

How to Build?
-------------

To initialize your local repository using the NinjaOS trees, use a 
command like this:

```bash
  repo init -u https://github.com/NinjaOS/manifest.git -b oreo
```
  
Then to sync up:
----------------

```bash
  repo sync -c -jx --force-sync --no-clone-bundle --no-tags
```
Finally to build:
-----------------

```bash
  . build/envsetup.sh
  lunch ninja_device_codename-userdebug
  mka shadow -jx
```
