# AAISP plugin for Munin #

[Munin](http://munin-monitoring.org/) plugin to graph [Andrews & Arnold / AAISP](http://aa.net.uk) broadband quota. Handles multiple lines associated with a single login.

It uses version 2 of AAISPs [CHAOS](https://support.aa.net.uk/CHAOS) API.

## Screenshots ##

x

## Plugin config ##

in /etc/munin/plugins-conf.d/aaisp:

```
[aaisp]
env.username aa11@a
env.password SomeLongPassword
```

## Setup ##

1. Install dependencies

2. Clone this repo

3. Set username and password in /etc/munin/plugin-conf.d

4. Symlink script

## Debugging ##

```
$ munin-run --debug aaisp config
$ munin-run --debug aaisp
```
