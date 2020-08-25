# gnirehtet-miui

This repository just contains patch files for the actual [gnirehtet][1] project.
The main goal is to remove `WRITE_SECURE_SETTINGS` from manifest file.
Because in Xiaomi MIUI, one has to enable USB Debugging Security Settings for
that permission and it requires to register with a MI account.

## How to use

Download the APK file from the [release page][2] and install in Android device.
Download the gnirehtet server from the [gnirehtet release page][3].
The rest is same as the actual [gnirehtet usage][4].

## Patch list

* 0001 - remove `WRITE_SECURE_SETTINGS` permission from `AndroidManifest.xml`.
* 0002 - update gradle build tools in `build.gradle` and `gradle-wrapper.properties` file.
* 0003 - update rust cargo crates depndencies in `Cargo.lock` file.

## Related links:

* [Main project: gnirehtet][1]
* [gnirehtet commit: Restrict GnirehtetControlService to privileged][5]
* [gnirehtet issue #5: Error: Requires permission android.permission.WRITE_SECURE_SETTINGS][6]
* [gnirehtet issue #40: gnirehtet can not run as service in Android][7]


<!-- Links -->
[1]: https://github.com/Genymobile/gnirehtet
[2]: https://github.com/Biswa96/gnirehtet-miui/releases
[3]: https://github.com/Genymobile/gnirehtet/releases
[4]: https://github.com/Genymobile/gnirehtet/blob/master/README.md
[5]: https://github.com/Genymobile/gnirehtet/commit/e7b84076a05effebf4aa2f47c9ad8ffff4fda382
[6]: https://github.com/Genymobile/gnirehtet/issues/5
[7]: https://github.com/Genymobile/gnirehtet/issues/40
