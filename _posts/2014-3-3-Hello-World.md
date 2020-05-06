---
layout: post
title: Housekeeper
---

Technology: python
Requirements:
- read configuration in json
- track git repositories updates
- install environment using docer with new repository version
- run tests

Environment setup in stages:
 - install tool
 - install tool configuration
 
Environment tools:
- OS ?
- git
- ssh keys setup
- curl
- python
- cmake
- repo
- jenkins
- clang

Flow:
1. Jenkins triggers HouseKeeper
2. HouseKeeper reads configuration
3. HouseKeeper checks git repositories
	1. If there is new version of tool HouseKeeper schedule Jenkins job with git repository address
	2. If there is no new version HouseKeeper exits.
