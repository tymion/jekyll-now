---
layout: post
title: HouseKeeper
---

*HouseKeeper* will ensure that all needed tool are up to date. Supervisor over digital environment.

Core *HouseKeeper* functionalities:
- JSON configuration
- enable to self-configure
- enable to setup environment from OS to application, from compilation to deployment

Environment setup:
- laptop for 3d designs: fast, stable, probably with Windows
- server with environment for android development with two phone devices and printer connected, NAS sertup

Server:
  1. Multiverse  supervisor executes and updates services, control resources and shares them to services
  2. Services - dockerized to be easily updated and tested
  2.1. 3DPrinterUniverseService - compiling Ender software, control printer, update sotfware
  2.2. WatchmanUniverseService - compiling Andoroid, watchman application, update devices
  2.3. StreamingUniverseService - shareing data, streaming content
  2.4. HouseKeeperUniverseService - tracks Universes dependencies, builds Universe and performs tests, build Multivers
  
  
TODO: create common flow for Universes i.e.: setup environemnt variables.
  
