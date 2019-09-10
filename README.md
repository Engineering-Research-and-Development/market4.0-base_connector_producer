# MARKET4.0 Base Connector Producer
The Base Connector Producer is an IDS connector, based on the IDS Base Connector, used in the Market4.0 project with the producer role.
The main objective is to communicate with the Base Connector Consumer in order to exchange data. The main components are:
* Apache ActiveMQ for data exchanging, supporting both openwire and ssl as the communication protocol
* Apache Camel for routes defining in order to forward the JMS messages to application endpoints

In order to use SSL, please use dummy certificates or creating new ones as illustrated by ActiveMQ documentation.

# How to install and run #
*** if you did steps 1 to 5 for the market4.0-base_connector_consumer skip these steps ***
1. Install the Virtal Box Version 6.0.10 r132072 (Qt5.6.2)
2. Download Ubuntu 18.04.3
3. Install the Ubuntu 18.04.3 on the Virtual Box
4. Run the Ubuntu under the Virtual box
5. Install in the Ubuntu next software:
	1. Java jdk( https://vitux.com/how-to-setup-java_home-path-in-ubuntu/ )
	2. Docker ( https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-18-04 )
	3. Git ( https://www.youtube.com/watch?v=TYnFm0zvy_s )
	4. docker-compose ( https://www.digitalocean.com/community/tutorials/how-to-install-docker-compose-on-ubuntu-18-04 )
6. Get the repository from the GitHub: sudo git clone https://github.com/Engineering-Research-and-Development/market4.0-base_connector_producer
7. Disable the firewall in the Ubuntu: 
	1. Install Firewall in the Ubuntu. 
		1. Set Profile: Public 
		2. Status: OFF
8. Run the projects: market4.0-base_connector_producer:
	1. Go to the folder where you get from the Git the project market4.0-base_connector_producer and run these commands:
		1. sudo docker-compose -f docker-compose.yml pull
		2. sudo docker-compose -f docker-compose.yml up
		
		

