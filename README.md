# maelstrom-ip

A simple perl script with low system resource usage that makes tcp connections to random IP address in order to obfuscate the IP connections seen by your ISP.

# Usage

Simply run `./maelstrom-ip` to start the script. <br />

To run as a service create `maelstrom-ip.service` at `/etc/systemd/system` and add the following: <br />

```perl
[Unit]
Description=maestrom-ip

[Service]
ExecStart=/path/to/maelstrom-ip

[Install]
WantedBy=multi-user.target
```


# Dependencies
perl >= 5.26.1 <br />
netcat >= 0.7.1 <br />


