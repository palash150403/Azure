# Azure IoT

## Azure IoT Explorer Installation Refs

```
https://github.com/Azure/azure-iot-explorer/releases
```
```
https://learn.microsoft.com/en-us/azure/iot/howto-use-iot-explorer
```

-   If installing a deb package then

```
sudo gdebi azure-iot-explorer_0.15.11_amd64.deb
```

-   Then Launch it

## Creating IoT Hub

![alt text](image.png)

## Adding Device

![alt text](image-1.png)

## Creating a Device

![alt text](image-2.png)

## Connecting rasspberry IoT simulator with iot device

#### Raspberry Web Simulator
```
https://azure-samples.github.io/raspberry-pi-web-simulator/
```

#### Copy the connection string

![alt text](image-3.png)

#### Replace the connection string with actual connection string 

![alt text](image-4.png)

#### Open azure explore and configure connection string here

![alt text](image-5.png)

#### Get Connection string from here

![alt text](image-6.png)

#### Start telemetory

![alt text](image-7.png)

#### Create Event Hub Namespcae

![alt text](image-8.png)

#### Create Event Hub

![alt text](image-9.png)

#### Configuring Event Hub 

![alt text](image-10.png)

![alt text](image-11.png)

![alt text](image-12.png)

![alt text](image-16.png)

![alt text](image-13.png)

-   Add Primary connection string of sas policy created to endpoint in iot explorer

![alt text](image-17.png)

![alt text](image-14.png)

![alt text](image-15.png)

#### Send D2C Messages to IoT Hub using VsCode

-   view Azure Azure iot hub in bottom left, click on tree dots.
-   Then select send D2C Messages to IoT Hub using VsCode

![alt text](image-18.png)

![alt text](image-19.png)

