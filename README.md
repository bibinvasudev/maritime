# maritime

Maersk has more than 4 lakh refer containers - how to manage and monitor the fleet and containers efficiently  in cost effective manner was the big challenge that they are facing for long time.
They have containers  going from the hottest place in Latin America to the coldest north of Alaska.

For this they are developing their own iot platform by integrating AT&T iot devices(AT1 devices created by AT&T) and IOT hub. For satellite communication they are using "Network in a box device" (NIB) devices developed by SSI(star solution international).
They call it as maersk industrial iot platform  where Azure and on premises flavor is available right now. This integrated platform will make sure that the real-time data is available in the data center.

Mainly the RCM device will send the real-time position , temperature and humidity inside the container and reset that based on the commands from the command center

[Detailed description - 
maersk industrial iot platform consist of iot hub. Iot hub help to inject the date from refer container devices. It has seamless integration with the azure function apps and on premises provisioning apps.
We can control these device with improved device management and provisional capability. This will provide a holistic view towards organization. We are getting the luxury of an online maintenance]

Advantages are -  we are  digitizing vessels and containers and removing paper work thus we are creating a collaborative port environment, so that all could exchange information digitally and making the container management more effective 

Our system will help 
1.	Safeguard your cargo from origin to destination.
2.	Providing the luxury of an online maintenance
3. disruption forecasting

NOTE- The end goal is to use data analytics to catch faults before they happen and  demand forecasting.


Detail- 
 Remote Container Management (RCM) allows you to monitor the conditions inside your container and make in-transit adjustments to ensure your cargo arrives in peak condition. Maersk monitor your cargo container from pickup to delivery, with detailed information on pull-down rates, temperature, energy, humidity and CO2 levels. You can also monitor your cargo 24/7 with our easy-to-use platform. If a setting deviates from your parameters, you’re notified automatically and we act quickly to rectify the issue. What’s more, GPS tracking enables us to quickly re-route cargo if the market situation changes. 

So, take control of your cargo. Enjoy end-to-end transparency and ensure your customers get better cargo quality on arrival.  

With Remote Container Management (RCM) you can monitor the conditions inside your container from the moment your goods are locked inside and till delivery at their final destination. In other words, our RCM system brings you peace of mind when shipping fresh, frozen or pharma cargo by eliminating the risk of unexpected surprises when your containers are opened upon arrival.


Majore data which is taking to the command center mainly consists :

1. Monitoring the light and humidity as it harms the contents
2. Door sensors to track where and when the container was opened and closed
3. Acoustic sensors to detect possible motion or theft in the container
4. Location and altitude sensors to track a containers precise location


On AUG 15, 2019 ESRI, CISCO, IBM, INTEL announced the developement of a similar system.

Esri technology is used to locate, track, map, and provide contextual geographic information. It brings real-time data integration and spatial analytics with map visualization, agile developer tools for web and mobile application development, along with a global library of geographic, demographic, and business data.

Intel’s Connected Logistics Platform provides near real-time supply chain visibility. It monitors the location, quality, and integrity of cargo at every stage of the supply chain, around the world. Companies, use this data to mitigate risk, improve operational efficiencies and reduce supply chain costs.

Cisco’s E-LAN, industrial routers provide Kinetic (Cloud) Services. It connects the Port’s sensor data and synthesizes it to automate port operations.  and



There is no direct open source option for these azure Services. But you can create a custom gateway very easily. Even azure documents talks about how to create custom IoT hub gateway.
As open source alternatives, I would recommend you to take a look at FIWARE community and EdgeX Foundry. FIWARE has a set of open source software components, called Generic Enablers (GEs), to help the development of future internet applications. You can see the following links about IoT and FIWARE:

Build your own IoT platform with FIWARE enablers
FIWARE enabling IoT big data ecosystems
IoT services enablement architecture
Edgex Foundry has a set of microservices that are being developed to help the integration between IoT devices and fog/cloud services. You can learn more reading the official site: https://www.edgexfoundry.org/ .



How to creta e a GIS application
https://www.earder.com/tutorials/postgis_geoserver_leaflet/


NAVIC - ISRO developed solution for fisherman boat tracking


Maersk devices used for Container tracking

        AT&T hardware RCD(remote connecting device)
        MCI( mearsk container industry) manufacturing WCD(Wireless communicating device)


Maersk has connected over 280,000 of its refrigerated containers to the AT&T network.
Each unit uses a remote container device (RCD) that has a 3G High Temperature SIM card, a GPS unit, a ZigBee radio and antenna, and multiple interfaces for connecting into the refrigerated container’s controller. 
The RCD can operate with two-way connectivity from just about anywhere in the world.

Here’s how it works. Each container has a monitoring device that collects data with sensors and sends it to a web portal.
Managers can view the location of containers for cargo owners. 
Back-office workers can easily find containers. 
Drivers have the tools to be more productive because they have more information about their next load to pick up.


They use eSIM - so it will automatically switch 


A recent report by TMR projects the value of global digital transformation of the maritime freight market to reach ~US$ 38.4 billion by 2027. 
IoTNowTransport.com notes that – “The digital transformation of maritime freight has drastically improved the efficiencies of marine freight companies by enabling the integration of artificial intelligence technologies, blockchain, Internet of Things, and robotics with shipping models.”


Implementation of a dedicated wireless network at sea ports can be used for digital transformation and to facilitate adoption of new digital technologies.
All sorts of applications can be deployed, from connecting port assets to monitoring harbor conditions, or connecting wireless surveillance to enabling self-driving vehicles.
One technology leading the way in implementing dedicated wireless networks is Private LTE. 
Industry leading supplier Qualcomm defines a Private LTE network as one tailored to serve a limited geographic area with optimized services using dedicated equipment.

The Private LTE Market size is set to exceed USD 11 billion by 2024; according to a new research report by Global Market Insights, Inc.

Satellite Internet access is Internet access provided through communications satellites. 
   Modern consumer grade satellite Internet service is typically provided to individual users through geostationary satellites that can offer relatively high data speeds,-
   with newer satellites using Ku band to achieve downstream data speeds up to 506 Mbit/s.

INPUT FROM MARITIME EXPERTS 
==========================

1. Now vessel crew used broadband internet facilities, watch televisions even make call
2. Some companies used Intellian broadband 
3. International maritime satellite is very popular, they have started all these facilities initially

Inputs regarding the tracking and monitoring in all ships


1. Manually sending - position, average speed etc. at Noon once a day
2. LRIT - long range , it’s going to flag state. i.e. India registered ships information goes to India
   So Indian will get information about its ships. LRIT is a part of  ISPS - international maritime security’s 
3. AIS- automatic identification system. For all ships AIS is mandatory
   AIS - ships data are automatically transmitting - gps position, course made good(effective course), effective speed, Geo heading, other static information like MMSI number maritime mobile station identification number , ship name, navigational status i.e. some time anchored, sailing, moved, crew numbers, body part how much inside water,  etc. and will transmit through the VHF range and its publicly available.
   All AIS receiver will get the nearest ships details
   AIS equipment is always on. 
   From Mid ocean also its transmitting
  
4. This is the new system that Maersk and all developed recently using GIS, IOT etc
    For REFER container delivery air temperature, written air temperature, container malfunction details, alarm status
   container international number(alpha numeric number)(container is sealed customs and we cannot open this only in emergency),origin, destination, cargo type
, up-normal dry container details, refer container bayplan -i.e. its position , wind speed, wind direction
sea water temperature, removed lashing dry container details  and other AIS information as well can be transmit to control room

5. For liner service 6 month schedule is fixed. SO no prediction is needed for scheduling as of now

----------------------

Digital transformation in the ocean shipping industry includes the ongoing deployment of sensors and tracking devices on refrigerated and dry shipping containers around the world. 
This smart container technology adoption enables greater visibility and management of goods being transported around the world.
A simple example is the shipment of bananas around the world. Shipping bananas requires refrigeration and controlled levels of oxygen and carbon dioxide while in a shipping container in order not to ripen prior to reaching the retailer. 
Smart container technology enables this control, tracking and monitoring to be possible.

While refrigerated containers (reefers) are being moved around on land, they are connected via commercial public mobile operator networks such as those offered by AT&T, Rogers, or Vodafone.
Each container has a smart device on it that uses mobile data services (GSM or LTE technology) to connect to the network. 
Once connected, it can share and transfer data to a centralized location where container owners can review real-time information and make decisions. 
They are also able to share this information with their customers and clients.

While the smart containers are at sea, there is no public mobile network coverage.
Without network coverage, the smart containers cannot be monitored remotely until it reaches the shore and reconnects.
Maritime shipping routes can be up to 20+ days and the only way to ensure a refrigerated container is working while at sea is to manually check it.
Large vessels can carry up to 10,000 containers so individually checking each unit becomes challenging.

Star Solutions’ Smart Container Solution enables each vessel the ability to have a private mobile network where it can continue to monitor, track and control the refrigerated units remotely during an ocean sailing.
With this private mobile network enabled at sea, shipping companies can offer its customers access to its smart container solution while on land and at sea.

The below diagram highlights the stages of mobile network coverage for goods being transported by smart containers. In stages where it states Public, it refers to the smart container being connected via the public mobile network (eg. AT&T, Rogers, Vodafone).
Private refers to the instances where a private mobile network on the shipping vessel connects to the smart containers locally and then enables data to be available to centralized resources.

===================

Collecting sensor data is nothing new in maritime transport. 
However, the global ship-to-shore connectivity – enabled by safe and secure Internet connection – makes it possible to gather data from an expanding array of onboard sensors and digitally distribute it throughout your logistics network.


Reference:-

https://www.starsolutions.com/company-blog/maritime-smart-container-solution/
https://customers.microsoft.com/en-us/story/757564-maersk-transportation-azure-iot
https://freightbro.com/maersk-line-the-leader-in-global-trade/


26-November-2019

https://www.universalcargo.com/how-can-smart-containers-help-shipping-companies/
https://www.msc.com/che/our-services/reefer-cargo
https://www.myshiptracking.com/ports/port-of-tilbury-in-gb-united-kingdom-id-421
https://www.vesselfinder.com/
https://www.marinetraffic.com/en/ais/home/centerx:-12.0/centery:25.0/zoom:4
https://www.marineinsight.com/know-more/top-8-websites-to-track-your-ship/

@aneesh
NIB crate a network. 

esims are not available in all. The Denmark sim will be in roaming for other place. less than 12nauticalmiles will switch to local GSM network
RCD communicate with NIB. 

November28.2019 updates

https://circuitdigest.com/article/arduino-vs-raspberryp-pi-difference-between-the-two

https://www.researchgate.net/publication/261343481_Intelligent_ports_based_on_Internet_of_Things/link/555e7a4e08ae8c0cab2c736e/download

Azure  iot suit and iot hub for developers - iot hub allow millions of devices to connect , though the web/mobile app we are saving this to Documentdb

Top Alternatives to Microsoft Azure IoT Hub are as follows:
Google Cloud IoT Core.
IBM Watson IoT Platform.
AWS IoT Device Management.
Oracle IoT Asset Monitoring Cloud.
Bosch IoT Suite.
SAP Cloud Platform for IoT.
AT & T IoT Platform etc.
