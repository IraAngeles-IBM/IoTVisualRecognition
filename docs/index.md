
# IoT Fire Alarm using Node-RED and IBM Visual Recognition 

This project is a how-to guide on using Node-RD and IBM Visual Recognition service to analyse an image and based on a trigger word then send a event command to IoT Device. In this example node-red is used to create an image upload form which sends the image to IBM Visual Recognition and trigger an iot device whenever fire is detected in the image.


1. Login/signup in to your [IBM Cloud Account](https://ibm.biz/BdYtcs)
2. Goto Catalog and create the following services:
    * Install [Node-RED](https://developer.ibm.com/tutorials/how-to-create-a-node-red-starter-application/)
     Note : Please follow the tutorial to install Node-RED in IBM Cloud

    * Create IBM Cloud Service [Internet of Things Platform](https://developer.ibm.com/tutorials/cl-mqtt-bluemix-iot-node-red-app)
Note : You need to create the A Platform Starter App,not Internet of things Platform service.I suggest you use the link above to quickly avoid confusion

    * Create IBM AI [Visual Recognition](create-visual-recognition-svc) service
    
    NOTE: You can skip steps 3,4 & 9

3. Goto connections tab and open IotF Service and Launch Watson Iot Platform
4. Navigate to Devices tab and Add Device
5. Once the Starter app is running,visit app url and configure Node-red
6. [Login to your node-red flows dashboard and import flow](import-flow.md)
7. [Update api key in the visual recognition node-red flow](update-flow)
8. Update the device details in IBM Iot device node {Optional}
9. [Visit node-red-url/upload and upload required image](upload-image.md)
10. Change the string inside includes from trigger action function to set a different trigger

