# rpi-domotic-diy

A DIY (Do It Yourself) domotic box based on : Raspberry Pi 2, InfluxDb, Grafana, MQTT and Node-Red

### Installation
Thanks to [InfluxDB, Telegraf and Grafana on a Raspberry Pi 2](http://www.aymerick.com/2015/10/07/influxdb-telegraf-grafana-raspberry-pi.html)

install go 1.5 using Go Version Manager
``` bash
$ bash < <(curl -s -S -L https://raw.githubusercontent.com/moovweb/gvm/master/binscripts/gvm-installer)
$ source /home/pi/.gvm/scripts/gvm
$ sudo apt-get install bison ruby-dev gcc
$ gvm install go1.4
$ gvm use go1.4
$ export GOROOT_BOOTSTRAP=$GOROOT
$ gvm install go1.5
$ gvm use go1.5 --default
```
install InfluxDb
``` bash
$ sudo dpkg -i ./package/influxdb_0.9.6_armhf.deb
$ sudo service influxdb start
```
install Grafana
``` bash
$ sudo dpkg -i ./package/grafana_3.0.0_armhf.deb
$ sudo service grafana-server start
```
and browse localhost:3000 to access Grafana UI

install broker mosquitto
``` bash
$ sudo apt-get install mosquitto
```
install Node-Red
``` bash
$ sudo apt-get install nodered
```
