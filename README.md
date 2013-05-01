# Chromium updater script for OS X

Update Chromium.app to the latest available trunk build.

* Reads the [LAST_CHANGE](https://commondatastorage.googleapis.com/chromium-browser-continuous/Mac/LAST_CHANGE)
  file generated by the [Chromium BuildBot](http://build.chromium.org).
* Uses [curl](http://curl.haxx.se/) to show a progress bar while downloading.
* Uses [rsync](https://rsync.samba.org/) to update the Chromium.app folder in-place.
* Retains zip files for the last three downloaded builds in case you need to revert.
