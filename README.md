# Client-Server-ZeroMQ
Simple example of the client-server pattern using ZeroMQ
(from distributed-systems.net)

### First, install ZeroMQ (on each machine):

    sudo apt update

    sudo apt install python3-zmq

### Or, with virtual environments (also on each machine -- only install pip3 and venv if not yet installed):

    sudo apt update
    sudo apt install python3-pip
    sudo apt install python3-venv
    python3 -m venv myvenv
    source myvenv/bin/activate
    pip3 install pyzmq

### Next, configure the IP address and port number of the publisher's machine in the constPS.py file

Note: Make sure that this repo is cloned in all the machines used for this experiment.

### Then, run the publisher and subscriber:

On the machine for which the IP address was configured:

    python3 publisher.py

On another machine:

    python3 subscriber.py

### Now, add other topics for in the publisher and create subscribers for the new topics.

    
