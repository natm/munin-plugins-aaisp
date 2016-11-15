# AAISP plugin for Munin #

[Munin](http://munin-monitoring.org/) plugin to graph [Andrews & Arnold / AAISP](http://aa.net.uk) broadband quota and sync rates. Handles multiple lines associated with a single login.

It uses version 2 of AAISPs [CHAOS](https://support.aa.net.uk/CHAOS) API.

## Demos ##

Live [demo install](https://munin.hw.esgob.com/broadband-day.html) with 3 lines.

## Screenshots ##

### Quota ###

Graph per line showing quota and data remaining:

![Screenshot](https://raw.github.com/natm/munin-plugins-aaisp/master/docs/quota_single_line_day.png) ![Screenshot](https://raw.github.com/natm/munin-plugins-aaisp/master/docs/quota_single_line_month.png)

Multiple lines on a single graph displaying data remaining:

![Screenshot](https://raw.github.com/natm/munin-plugins-aaisp/master/docs/quota_multiple_lines_combined_day.png) ![Screenshot](https://raw.github.com/natm/munin-plugins-aaisp/master/docs/quota_multiple_lines_combined_month.png)

### Sync rate ###

A single line displaying down and upstream sync:

![Screenshot](https://raw.github.com/natm/munin-plugins-aaisp/master/docs/syncrate_single_day.png)

Multiple lines, downstream rates (upstream graph also produced):

![Screenshot](https://raw.github.com/natm/munin-plugins-aaisp/master/docs/syncrate_downstream_combined_day.png)

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
