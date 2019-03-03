# Fluentd
Fluentd installation for Ubuntu:

# Download package
curl -L https://toolbelt.treasuredata.com/sh/install-debian-stretch-td-agent3.sh | sh
cd /var/log/nginx

#change permission
sudo chmod -R 777 grid

#change configuration
cd /etc/td-agent
sudo mv td-agent.conf td-agent.orig
cd /opt/td-agent/usr/sbin

#Install reguired Plugins
sudo ./td-agent-gem install fluent-plugin-record-transformer

