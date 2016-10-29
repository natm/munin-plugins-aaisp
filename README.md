# AAISP plugins for Munin #

[Munin](http://munin-monitoring.org/) plugin to graph [Andrews & Arnold](http://aa.net.uk) / AAISP broadband quota.

It uses version 2 of AAISPs [CHAOS](https://support.aa.net.uk/CHAOS) API.

Currently graphs total quota and that remaining. Handles multiple lines associated with a single login.

## Screenshots ##

x

## Plugin config ##

in /etc/munin/plugins-conf.d/aaisp:

```
[aaisp]
env.username aa11
env.password SomeLongPassword
```

## Setup ##

1. Install dependencies

2. Clone this repo

3. Set username and password in /etc/munin/plugin-conf.d

4. Symlink script
