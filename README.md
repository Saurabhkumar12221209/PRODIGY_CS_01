 Python 3 Network Packet Sniffer
Python Version OS CodeFactor Grade License

Reddit Discord Twitter

A Network Packet Sniffer developed in Python 3. Packets are disassembled as they arrive at a given network interface controller and their information is displayed on the screen.

This application depends exclusively on the NETProtocols library (also developed and maintained by EONRaider) from version 2.0.0 and above and can be run by any Python 3.8+ interpreter.

Demo
sniffer_demo

Running the Application
I. Development Mode
Simply clone this repository with git clone, install the dependencies and execute the sniffer.py file.

user@host:~$ git clone https://github.com/EONRaider/Packet-Sniffer.git
user@host:~$ cd Packet-Sniffer
user@host:~/packet-sniffer$ pip install -r requirements.txt <--or--> poetry install
user@host:~/packet-sniffer$ sudo python3 packet_sniffer/sniffer.py
The sudo command is required due to the use of socket.SOCK_RAW, which needs administrative privileges to run on GNU/Linux. Notice that the existence of dependencies may require the execution of the interpreter contained in the virtual environment in which the dependencies have been installed (if you use one), instead of just using the system interpreter.

II. (Optional) Build the binary
Use the build.py file to compile your own binary with the PyInstaller package. You just need to install all dependencies and build. Dependency management works with both Poetry (recommended) and Virtualenv.

<-- Install dependencies as shown above in Step I -->
user@host:~/packet-sniffer$ python3 build.py
Usage
sniffer.py [-h] [-i INTERFACE] [-d]

Network Packet Sniffer

optional arguments:
  -h, --help            show this help message and exit
  -i INTERFACE, --interface INTERFACE
                        Interface from which packets will be captured (monitors
                        all available interfaces by default).
  -d, --data            Output packet data during capture.
Legal Disclaimer
The use of code contained in this repository, either in part or in its totality, for engaging targets without prior mutual consent is illegal. It is the end user's responsibility to obey all applicable local, state and federal laws.

Developers assume no liability and are not responsible for misuses or damages caused by any code contained in this repository in any event that, accidentally or otherwise, it comes to be utilized by a threat agent or unauthorized entity as a means to compromise the security, privacy, confidentiality, integrity, and/or availability of systems and their associated resources. In this context the term "compromise" is henceforth understood as the leverage of exploitation of known or unknown vulnerabilities present in said systems, including, but not limited to, the implementation of security controls, human- or electronically-enabled.

The use of this code is only endorsed by the developers in those circumstances directly related to educational environments or authorized penetration testing engagements whose declared purpose is that of finding and mitigating vulnerabilities in systems, limiting their exposure to compromises and exploits employed by malicious agents as defined in their respective threat models.

About
A Network Packet Sniffing tool developed in Python 3.

Topics
packet-sniffer network-programming tcp-ip ethical-hacking pentesting-tools
Resources
 Readme
License
 AGPL-3.0 license
 Activity
Stars
 747 stars
Watchers
 23 watching
Forks
 99 forks
Report repository
Releases 5
v2.1.0
Latest
on Jul 8, 2022
+ 4 releases
Contributors
5
@EONRaider
@jdevries3133
@zahash
@sammichaels
@folkertvanheusden
Languages
Python
100.0%
Footer
© 2025 GitHub, Inc.
Footer navigation
Terms
Privacy
Se
