Node.JS library for Broadlink RM2 IR controllers
===============================================

A Node.JS module for controlling IR controllers from [Broadlink](http://www.ibroadlink.com/rm/). At present, only RM Pro (referred to as RM2 in the codebase) devices are supported. There is currently no support for the cloud API.
This module was re-implemented using javascript from [python-broadlink](http://github.com/mjg59/python-broadlink).

Example use
-----------

Please see test.js for temperature checking and ir learning example.

Running on Windows
--------
in order to run on windows you need to:
1) provide your internal network ip prefix
or your ip in a global environment called `IP_PREFIX`
2) find your broadcast ip by calling ipconfig as described [here](https://documentation.progress.com/output/ua/OpenEdge_latest/index.html#page/gsins/determining-the-broadcast-address.html)
3)set global environment called `BROADCAST_ADDRESS` with your broadcast adress
####for example run
```bash
$ IP_PREFIX=10.0.0.10 BROADCAST_ADDRESS=10.0.0.255 node yourApp.js
```
