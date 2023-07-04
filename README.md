<h1>Mosquitto MQTT Broker<h1>

<h2>What is it?<h2>
MQTT is a lightweight, publish-subscribe, machine to machine network protocol for message queue/message queuing service.
It is designed for connections with remote locations that have devices with resource constraints or limited network bandwidth, such as in the Internet of Things.

<h2>Installation<h2>
In order to start up Mosquitto via Docker Compose, just run "docker-compose up -d" from root directory of this repository.

<h2>How to use it?<h2>
To publish a message simply run this command: <br>
mosquitto_pub -h localhost -p 1883 -m "your message" -t "topic name"
<br>
<br>
And for subscribing and receiving messages from a topic: <br>
mosquitto_sub -h localhost -p 1883 -t "topic name"
