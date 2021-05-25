# Patches
##### unpatch.bsdiff
The most commonly distributed Windows NT 3.1 ISO has modified setup files, apparently in an attempt to make it installable with newer processors. Unfortunately, this had the side effect of making it uninstallable in emulators of older processors where it should otherwise work, like PCem. Since I do not have a clean copy of the ISO, I undid the changes as best as I could and made a patch.

The ISO image in question has an md5sum of _f20834ca9978a5a181c120145f77d7ea_ and a sha1sum of _edb096d96a69c74395967dd5e05dfe1a5aa4cd57_. If I happen to find a clean original ISO, I will remove this patch or replace it with a patch to restore the crappy one to the good one.


Usage:

bspatch en_winnt_3.1.wks.iso fixed.iso unpatch.bsdiff

##### unpatch.xdelta

Same as above, but with xdelta.

Usage:

xdelta patch unpatch.xdelta en_winnt_3.1.wks.iso fixed.iso
