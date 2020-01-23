# tumblr_backup

A port of the popular tumblr_backup python script to Python 3, since Python 2 has finally kicked the bucket.

Usage parameters are identical to the old script. Doesn't rely on anything outside the stdlib, although youtube-dl and pyexiv2 are highly useful.

License is GPLv3, just like the original.

## Fixes applied

This is more or less the amount of steps that it took to convert this python 2 script to python 3.

* Ran 2to3
* Fixed content-type check in API requests
* Removed a pointless decode
* Fixed time.mktime
* Fixed hexdigest generation for the tag index (this is broken in the python 2 script, fixed in this one).

## Notes

The core codebase is completely unchanged. In my personal opinion, the code could use a complete overhaul from scratch, it's quite a mess to read. This was purely a hacked together fix to get the script working again.