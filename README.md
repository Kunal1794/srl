**##Physical Topology**

![image](https://github.com/Kunal1794/srl/assets/54974430/70226a36-ed39-4c8d-afce-d2e1f3d33082)

## deploy the lab
containerlab deploy DC1.yaml

## destroy the lab
containerlab destroy DC1.yaml

## Accessing the network elements
After deploying the lab, the nodes will be accessible. To access a network element, simply use its hostname as described in the table displayed after execution of the deploy command.

ssh admin@IP
telnet IP 5000 (Also for SROS)
cred : admin/admin (SROS) admin/NokiaSrl1!(SRL)

## The Linux CE clients don't have SSH enabled. In order to access them, use `docker exec`.**

docker exec -it clab-evpn-client1 bash

## Configuration
All nodes come preconfigured thanks to startup-config setting in the topology file. Those configuration files can be found in [config]

## L2 EVPN Topology

![image](https://github.com/Kunal1794/srl/assets/54974430/f1e8d44f-97f8-466d-ae2b-f5d8df98bac8)


## L3 EVPN Topology

![image](https://github.com/Kunal1794/srl/assets/54974430/084cf2f0-470c-40dc-a1ae-9547ae1cd76e)


