# maelstrom-ip

A simple perl script with low system resource usage that makes tcp connections to random IP address in order to obfuscate the IP connections seen by your ISP.

# Usage

Simply run `./maelstrom-ip` to start the script. <br />

To run as a service create `maelstrom-ip.service` at `/etc/systemd/system` and add the following: <br />

`[Unit]
Description=maestrom-ip

[Service]
ExecStart=/usr/bin/maelstrom-ip

[Install]
WantedBy=multi-user.target`


# Dependencies
perl >= v5.26.1 <br />
netcat >= v0.7.1 <br />


