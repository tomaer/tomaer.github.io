---
title: Backup My Macbook Pro with Docker timemachine
date: 2017-05-09 22:14:38
tags:
---

# 
```
docker run -h timemachine --name timemachine --restart=unless-stopped -d -v ~/nas/timemachine:/timemachine -p 548:548 -p 636:636 -d tomaer/timemachine:raspberrypi
docker exec -ti timemachine add-account username password point [size]
defaults write com.apple.systempreferences TMShowUnsupportedNetworkVolumes 1
```
