---
title: "journalctl cheat cheet"
date: 2022-05-11
menu: "CLI"
weight: 1 

---
# Journalctl cheatsheet
You got to love systemD

#### See all
```
journalctl
```

#### Follow stream of logs
```
journalctl -f
```

### Read boot messages
```
journalctl -b 
```

### Show reboots
```
journalctl --list-boots
```

### Timerange of log
```
journalctl --since "1 hour ago"
```

or
```
journalctl --since "2 days ago"
```

or between
```
journalctl --since "2022-01-01 00:15:00" --until "2022-01-01 12:00:00"
```

### Show log of unit file
```
journalctl -u gitlab-runner 
```

### Tail log of unit file
```
journalctl -u gitlabrunner -f
```
