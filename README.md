x# cfd18
CodeFunDo 2018

A solution to allow for survivor mapping/survey in city blocks immediately after natural disasters.

####### PROBLEM STATEMENT #####

What is common to every disaster? The loss of communication facilities.
Telecom towers are an essential utility, rather than some luxury service. Most rescue efforts often take weeks because entire buildings must be scavenged randomly. Moreover, we have anxious people outside the disaster zone who sit impatiently, waiting for news of their loved ones. Take one minute, and try to understand just how convenient it would be disaster relief systems could take mobile phones, or even fixed landline telephones, into account as sources of information instead of having to rely on the oft chance that someone would be able to contact them.

####### THE SOLUTION ##########

While cell towers and other relatively heavy equipment is down, mobile phones and laptops are NOT. They can be pressed into service, preferably immediately. More importantly, they can be used to tag people or groups of people for atleast the first first of the incident.

We can establish a peer-to-peer network based on WiFi Direct technologies to communicate locations of masses of people. This allows for the following benefits:
1. Rescue teams and the government gets quick, dirt-cheap survey of the ground situation. 
2. People can be 'marked as safe' or 'in  need of urgent medical assistance'.
3. The community gets to identify safehouses :  people with stocks of food, or department stores, etc. which are providing much needed food and other supplies till relief teams arrive and setup camp.
4. Important messages can be sent to the outside world. AMBER Alerts can be sent to the people stuck in disaster-hit areas.
5. This is extremely economical, and its efficiency improves as it scales up.

####### TECHNOLOGIES USED ##########

The exact technologies used would be derived from:

1. Peer-to-peer networking systems, like the BitTorrent protocols : Since phones need to communicate and pass on messages.

2. WiFi Direct and Bluetooth Technologies :  Like ShareIT and other applications using such technologies, we can process large amounts of data very quickly using such technologies. The expectation is that many phones close together would be able to connect and transmit/accumulate data up to a point where one such node reaches (a) the authorities (b) the telecom systems, when this data can be uploaded to the authorities.

3. Bing Maps :  The data received this way is uploaded and laid out on top of Bing Maps to get an assessment of survivors in city blocks. Along with altitude data, this can be used to model the damage patterns.

4. Computing services :  Using models of the disaster and expected survivor rates in various areas, it is a matter of using previous datasets about population trends in these regions to make guesses about the type of rescue efforts needed. This can help prioritise relief efforts towards regions requiring urgent medical assistance or supplies, while allowing them to provide necessary support to areas with relatively little damage or a constant stream of short term supplies. This requires computing power. lots of it. 

5. If possible, we can have drones or helicopters with higher power wifi devices sweep the city. This would greatly enhance the amount of data collected this way.

######### WORKING ###################

1. An application that shall be turned on whenever disaster warning alerts are received by user.

2. The application begins to track user location at regular intervals, and uploads it to Azure.

3. If connectivity is lost for extended periods of time, like 30 minutes, it goes into disaster mode. The user is asked for inputs for sometime. A personal wifi network is created and broadcast. It also scans for other nearby networks.

4. Should the user be able to access the device, they can input their health condition( fine,need assistance), food supply situation, number of people, condition of present housing(broken, fine, waterlogging, building collapse imminent, etc.)

5. These details are broadcast over Wifi networks. If other devices with the app are nearby, contents of both devices shall be exchanged. This way, both have two sets of details now. 

6. This process goes on and on till a lot of devices have a lot of data on each. Eventually, the data itself has travelled across a lot of distance by these "hops". 

7. Some device is able to find a network connection. It uploads all of this data to the cloud. Authorities now possess locations of a huge set of people. 

8. Authorities redirect resources to help people in this dataset.

############# PERSONAL PROFICIENCY ################

I know basic C++. I know I need help to implement such technologies. But I feel this has potential. Thank you for reading this.
