---
name: bl
description: Simple hosts blacklist script in bash
type: code
author: Evan Edwards
category: utility
---


# bl

`bl [CMD [CMD]...]`

Manages blacklist line in /etc/hosts.


# Demonstration

![Screen Recording](bl-demo.gif)


# Installation

1. Copy `src/bl` to some place like `$HOME/.local/bin`
2. Add the following two lines to `/etc/hosts`:

```
#!bl key:domain key2:domain2
127.0.130.1 blacklisted
```

Optional: The file and ip address can be altered by editing the script.


# Operations

```
  key     - Same as +key
  +key    - Add domain corresponding to available key
  -key    - Remove domain corresponding to available key
  @domain - Add domain
  ^domain - Remove domain
```


# Legal

Copyright 2024 Evan Edwards <evan@cheshirehall.net>

Released under an open source MIT License.  See LICENSE for details.
