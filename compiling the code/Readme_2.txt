zlog.conf -> Copy this into /etc path of the switch and ubunutu machine. This is required to set the logging library.
Monitor-Automata-Source-Code/Monitor-automata   --> Contains the first version of the source code without Timer grouping taken from the repo
Monitor-Automata-Source-Code/Monitor-automata-Backup   --> Contains the first version of the source code with Timer grouping taken from the repo.


monitoring-model --> Contains data-modeling files which should be eventually merged with the contents of the model folder present @ OFCONFIG/Mon-model/server-src/model
To merge, each time after generating a data-model, use a file comparator such as Meld Diff Viewer.

ostinato-bin-win32-0.8 -> Contains the Traffic Generator application.
To use the traffic generator, follow the below steps on a windows machine:
1. Run drone.exe as an administrator
2. Run ostinato.exe as an administrator as well.
3. Select any of the sessions by clicking on File-> Open Session : All the sessions are ending with the file name *.ossn.
4. It will have atleast one flow  already present. 100flows_using_one_stream.ossn is a good example to use.
It sends VLAN tagged (with VLAN ID-10 as expected by the Accton AS5712 switch) packets with source IP 50.0.0.1 to 50.0.0.N where N can be configured from the tool and the destination IP will be always 20.1.1.2

https://userguide.ostinato.org/  for more information on Ostinato.
Important to Click on APply button before starting the traffic on a port.


IPTABLES_FORWARD COMMANDS  --> How to setup the internet to connect the switches to internet.
