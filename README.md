# rootlessJB5
rootlessJB5 is the latest release of rootlessJB, this time supporting iOS 15.0 and 15.0.1. With the release of iOS 15, Apple made some significant changes to the root filesystem and how it reacts to unauthorized changes. Due to these measures, any unauthorized modifications of the root filesystem will cause a kernel panic, causing your device to immediately reboot. Until a solution or workaound has been discovered to circumvent these security measures, iOS 15 users will have to use a rootlessJB, which doesn't directly modify the root filesystem.

## Saily Implementation
- Saily is bundled with rootlessJB5 and will automatically be installed.
- Saily is currently the only supported package manager that is capable of running on a rootlessJB.
- Not all packages will work with rootlessJB's tweak injection by default.
- Please be patient and wait for developers to update their packages.
- Sideload with AltStore!
- [Saily ipa](SailySandBoxed.ipa "Saily.ipa")

## Installation
Installing rootlessJB5 is as simple as downloading the rootlessJB5.ipa file from the Releases section and sideloading it with AltStore.

## Important Usage Notes
- Binaries are located in: /var/containers/Bundle/iosbinpack64
- Jailbreak structs can be found at /var/containers/Bundle/tweaksupport/
- Symlinks include: /var/LIB, /var/ulb, /var/bin, /var/sbin, /var/Apps, /var/libexec
- The root filesystem will be kept read only, but don't modify /var, as this will cause problems.

## So what those scripts do?
- unSign.sh keeps Apple away from tracing our expensive certs.
- unPack, Clean, and Pack are used for those binpacks.

## What's next?
- fixmMap is coming for App Store apps.
- Adding support for remounting the user filesystem, but nothing will be wrote to /. So unless you put Cydia.app in /Applications you should be fine. You can also disable it.
- Full Substitute, Substrate, & libhooker implementation
- New Tweak Inject (Current one causes the device to kernel panic when installing a tweak from Saily)


Thanks to: 

* Jake James
* Ian Beer
* Brandon Azad
* Brandon Plank
* Jonathan Levin
* IBSparkes
* Sam Bingner
* Sammy Guichelaar
* Ned Williamson
* Umang Raghuvanshi
* Tanay Findley
* Lakr Aream
* Brecken Lusk
