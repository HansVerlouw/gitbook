# readme

## Prerequisites

### RabbitMQ

Start a RabbitMQ docker container. See https://git.geodan.io/icms/docs/icms-doc/wikis/docker for more info\
Be sure the guest account (guest/guest) is active and has permissions on the `/` virtual host (See the _Admin_ tab in RabbitMQ)\
The AMQP address should be: 192.168.99.100:5672 (this is the default port)

### Node.js

[Node.js](https://nodejs.org) is required to run this example. (v8.11.1 is used when testing this example)

## Installation

```powershell
# Clone the project to your local machine
git clone git@git.geodan.io:icms/icms-system-engineering.git

# Browse to this folder
cd examples/rabbitmq-amqp

# Install the node modules
npm install

# Start a consumer
node .\receive.js

# Open a new terminal window and run the following command to produce a hello world message
node .\send.js
```

More info: https://www.rabbitmq.com/tutorials/tutorial-one-javascript.html
