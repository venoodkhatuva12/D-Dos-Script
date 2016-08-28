# D-Dos-Script
Install DDoS Deflate To Block DDoS Attack....
(D)DoS Deflate is a lightweight bash shell script designed to assist in the process of blocking a denial of service attack. It use the command below to create a list of IP addresses connected to the server, along with their total number of connections.

netstat -ntu | awk ‘{print $5}’ | cut -d: -f1 | sort | uniq -c | sort -n

Features of (D)DoS Deflate

Configuration file: /usr/local/ddos/ddos.conf

To whitelist IP address, use /usr/local/ddos/ignore.ip.list.

It is having a feature to unblock IP addresses automatically after a preconfigured time limit.

You can execute the script at a chosen frequency.

You will get email alerts when IP addresses are blocked.

Installation

wget http://www.inetbase.com/scripts/ddos/install.sh

chmod 0700 install.sh
./install.sh
Uninstallation

wget http://www.inetbase.com/scripts/ddos/uninstall.ddos

chmod 0700 uninstall.ddos
./uninstall.ddos
Script to check No of connected ip’s.

sh /usr/local/ddos/ddos.sh

Restart DDos Deflate

sh /usr/local/ddos/ddos.sh -c

More info:

Its possible for you to edit the script and modify it according to your requirement.

To whitelist an IP addresses just add it to /usr/local/ddos/ignore.ip.list
Main Configuration file is /usr/local/ddos/ddos.conf
IP addresses are automatically unblocked after a default time limit (default: 600 seconds)
The script can run at a chosen frequency as set in the configuration file (default: 1 minute)
You can set the alerts in configuration file to receive email alerts when IP addresses are blocked.
