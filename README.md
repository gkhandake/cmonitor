[![Build Status](https://travis-ci.com/f18m/nmon-cgroup-aware.svg?branch=master)](https://travis-ci.com/f18m/nmon-cgroup-aware)

# nmon-cgroup-aware

Fork of Nigel's performance Monitor for Linux, adding cgroup-awareness. Makes it easy to monitor your LXC/Docker container performances.

NOTE: this is actually a fork of "njmon", not "nmon". njmon provides no interactive mode (often useless inside containers!) and is a more modern tool that produces a JSON output that can be used together with tools like InfluxDB (https://www.influxdata.com/) and Grafana (https://grafana.com/).


## How to use

Install and launch njmon inside your container; e.g. if you use an LXC container
based on a Centos/RHEL/Fedora distribution you can log into the container and run:

```
yum copr enable f18m/nmon-cgroup-aware
yum install -y nmon-cgroup-aware
njmon -C -s3 -f -m /home
```

## Links

- Original project: http://nmon.sourceforge.net
- Other forks: https://github.com/axibase/nmon
