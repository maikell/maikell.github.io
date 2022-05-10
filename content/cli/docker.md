---
title: "Docker cheat sheet"
date: 2022-04-27T16:35:53+02:00
---

# Docker Cheat sheet

#### stop all containers
```
docker stop all containers #  docker stop $(docker ps -aq)
```

### Remove all unused containers, networks, images (both dangling and unreferenced), and optionally, volumes. 
```
docker system prune  -f
```
-f = Do not prompt for confirmation
