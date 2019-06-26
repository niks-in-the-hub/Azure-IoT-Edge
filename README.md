# Azure-IoT-Edge

Azure IoT Edge was recently released as a generally available service.
With the edge module, it is possible to deploy applications from azure to an edge device.

However, I would like to first create a Data pipeline for the data generated from my edge device using azure resources, before trying to deploy cloud -> edge.

My basic configuration for this mini project is the following

Edge

1. Raspberri 3B+
2. Grove interface board
3. Grove sensor kit
4. Raspbian OS image on the micro SD card
5. Azure CLI (configured with Docker). Azure CLI cannot be installed natively as in windows. It is setup inside a container. 

Each time one wishes to start Azure CLI, the docker is started first with all following  CLI commands having the prefix "docker exec"

cloud

Setup the following resources on a trial subscription

1. Event Hub
2. Table storage
3. Azure function App
4. (IoT Edge module)