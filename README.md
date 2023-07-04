Mosquitto MQTT Broker

What is it?
MQTT is a lightweight, publish-subscribe, machine to machine network protocol for message queue/message queuing service.
It is designed for connections with remote locations that have devices with resource constraints or limited network bandwidth, such as in the Internet of Things.

Installation
In order to start up Mosquitto via Docker Compose, just run "docker-compose up -d" from root directory of this repository.

To publish a message simply run this command:
mosquitto_pub -h localhost -p 1883 -m <your message> -t <topic name>

And for subscribing and receiving messages from a topic:
mosquitto_sub -h localhost -p 1883 -t <topic name>
