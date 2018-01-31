Scripts for use with the load testing tool WRK
==============================================

multiplepaths.lua
-----------------

This file was modified from https://github.com/timotta/wrk-scripts/blob/master/multiplepaths.lua

The difference is that shuffling is not used, so the order in which paths are requested is the order that they are in the file. If you need shuffling, please use the original version instead.

You have to create a paths.txt file with one path per line in the current working directory.

Then, call wrk with the following params assuming that multiplepaths.lua is in the current directory (and any other that you need):

```
wrk -s multiplepaths.lua https://some-ip-or-address-goes-here
```
