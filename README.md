This script will remove all existing close-wait connections on the server

## Debian
```
$ apt-get install libnet-rawip-perl libnet-pcap-perl libnetpacket-perl
```

## CentOS
```
yum install libpcap-devel
perl -MCPAN -e 'install NetPacket'
perl -MCPAN -e 'install Net::Pcap'
perl -MCPAN -e 'install Net::RawIP'
```

## Usage
```
$ ./kill_close_wait_connections.pl
```

To install permanently you can do the following:

```
$ mv kill_close_wait_connections.pl /usr/bin/kill_close_wait_connections
$ chmod +x /usr/bin/kill_close_wait_connections
$ kill_close_wait_connections
```
