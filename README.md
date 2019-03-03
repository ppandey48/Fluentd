# Fluentd
Fluentd installation for Ubuntu:

# Download package
curl -L https://toolbelt.treasuredata.com/sh/install-debian-stretch-td-agent3.sh | sh
cd /var/log/nginx

# Change permission to read the log directory
sudo chmod -R r+w dir

# Change configuration
cd /etc/td-agent
sudo mv td-agent.conf td-agent.orig
cd /opt/td-agent/usr/sbin

# Install reguired Plugins
sudo ./td-agent-gem install fluent-plugin-record-transformer

