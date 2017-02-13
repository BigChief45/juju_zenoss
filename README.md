# Zenoss Core Juju Charm
This charm allows easy deployment of Zenoss Core 4.2.5 to your Juju environment.

**NOTE:** This charm has only been tested with Juju 1.25

## Installation & Deployment

Clone the repository to your local charm repository. Assuming that your local charm repository is located in `/home/$USER/charms/`:

```
cd charms/trusty
git clone https://github.com/BigChief45/zenoss-charm.git
```

Deploy locally using Juju:

`juju deploy --repository=/home/$USER/charms local:trusty/zenoss --debug`

## Zenoss Core 4 Debian Package

Currently the Zenoss Core 4.2.5 Debian package is obtained from [SourceForge](https://sourceforge.net/projects/zenossforubuntu/files/zenoss-core-425-2108_03c_amd64.deb). This location could change or the link could become broken in the future.

However you can easily change the package retrieval location by changing the `COREDIR` variable's value in `hooks/install`.
