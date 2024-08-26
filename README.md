# OVHcloud Nagios Plugins

The OVHcloud Nagios Plugins is a set of scripts designed to be executed by
Nagios, locally or via NRPE, to monitor various softwares.

# Installation

```
RELEASE=0.0.1
curl -sL https://github.com/ovh/ovh-nagios-plugins/archive/refs/tags/${RELEASE}.tar.gz | tar xvpzf - -C /opt
ln -s /opt/ovh-nagios-plugins-${RELEASE} /opt/ovh-nagios-plugins
```

# Configuration

Examples of configuration can be found in the [docs](docs) directory.

# Hacking

```
git clone https://github.com/ovh/ovh-nagios-plugins.git
cd ovh-nagios-plugins
python3 -m venv venv
. venv/bin/activate
pip install -r requirements.txt
```

You've developed a new cool feature? Fixed an annoying bug? We'd be happy
to hear from you!

Have a look at
[CONTRIBUTING.md](https://github.com/ovh/ovh-nagios-plugins/blob/main/CONTRIBUTING.md).

# Related links

 * [Contribute](https://github.com/ovh/ovh-nagios-plugins/blob/main/CONTRIBUTING.md)
 * [Report bugs](https://github.com/ovh/ovh-nagios-plugins/issues)
 * [Get latest release](https://github.com/ovh/ovh-nagios-plugins/releases)
