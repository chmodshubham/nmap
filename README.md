# nmap

Here are some common Nmap commands that can be used to explore a network:

### Basic host discovery:
```
nmap -sP <network address>
```
This command sends an ICMP ping request to each host on the specified network address to determine which hosts are up and running.

### Port scanning:
```
nmap -p <port range> <target>
```
This command scans the specified port range on the target host. For example, to scan the first 1000 ports on a host at IP address 192.168.1.1, you would run:
```
nmap -p 1-1000 192.168.1.1
```
### OS detection:
```
nmap -O <target>
```
This command attempts to determine the operating system running on the target host based on the way it responds to Nmap probes.

### Service detection:
```
nmap -sV <target>
```
This command attempts to determine the services running on the target host and their version information.

### Full port scan:
```
nmap -p- <target>
```
This command scans all ports on the target host. This can be a time-consuming process and is not recommended for large networks.

### Scripted scans:
```
nmap -sC <target>
```
This command runs the default Nmap script scan, which uses a collection of scripts to perform common tasks like banner grabbing, vulnerability detection, and service enumeration.

### Aggressive scanning:
```
nmap -A <target>
```
This command enables aggressive scanning, which includes OS detection, version detection, script scanning, and traceroute.

These are just a few examples of the many Nmap commands that can be used to explore a network. Nmap is a powerful tool, but it should be used carefully and with permission from the network owner to avoid any legal or ethical issues.
