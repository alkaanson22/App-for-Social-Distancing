# SocialDistancingApp
## How AI can solve some of the problems posed by Covid , like AI@Covid Solutions
### Team : T850
Alka Anson 

Neomi Sony

Shebon Shajan

Nikita Mathew
## Introduction
The world is currently fighting one of the greatest battles of humanity - the Coronavirus battle. The World Health Organisation (WHO) has declared the COVID-19 a pandemic. A pandemic is defined as "occurring over a wide geographic area and affecting an exceptionally high proportion of the population". A global coordinated effort is needed to stop the further spread of the virus. Doctors, scientists, healthcare workers, and many others are putting their hearts and souls into finding a solution to end this pandemic. As this pandemic is still tremendous in many countries, the world after the pandemic will witness several major trends. As the world battles against COVID-19, every ounce of technological innovation utilized to fight this pandemic brings us one step closer to overcoming it. Artificial intelligence is playing a key role in better understanding and addressing the COVID-19 crisis. AI technology has been introduced already across various sectors. It is being used for analyzing medical data, preparing treatment plans, contact tracing, analyzing transmission rates, drug development, and detecting hotspots. AI is adept at identifying patterns from big data, and this piece will explain how it has become one of humanity's ace cards in handling this crisis. AI tools and techniques can help policymakers and the medical community understand the COVID-19 virus and accelerate research on treatments.
## Problem Statement:

COVID-19 spreads mainly among people who are in close contact (within about 6 feet) for a prolonged period. Spread happens when an infected person coughs, sneezes, or talks, and droplets from their mouth or nose are launched into the air and land in the mouths or noses of people nearby. The droplets can also be inhaled into the lungs. Recent studies indicate that people who are infected but do not have symptoms likely also play a role in the spread of COVID-19. Since people can spread the virus before they know they are sick, it is important to stay at least 6 feet away from others when possible, even if you—or they—do not have any symptoms. Social distancing is especially important for people who are at higher risk for severe illness from COVID-19 and it helps limit opportunities to come in contact with contaminated surfaces and infected people outside the home.


The best way to follow social distancing is by following the guidance from local public health authorities wherever you live, preparing for transportation before you go out, wearing a mask and limiting  contact when running errands, choosing safe social activities, keeping distance at events and gatherings. In addition to practicing everyday steps to prevent COVID-19, keeping space between you and others(minimum 6 feet) is one of the best tools we have to avoid being exposed to this virus and slowing its spread in communities. Everyone has a role to play in slowing the spread and protecting themselves, their family, and their community. Through our app we would like to help enforce the social distancing norms in an easy, economical  and user friendly way.

## Solutions:
To address the above mentioned problem a Mobile App can be developed comprising of the following features:

### I.	Alert using bluetooth signals 
An alert beep is used to warn users of the proximity of any Covid patients nearby. The distance can be measured using bluetooth signal strength which roughly provides the distance upto few metres.
### II.	Using Intelligent Video Surveillance
When organizations leverage intelligent video surveillance, they can configure rule-based alerts to trigger notifications when certain predetermined threshold quantities of people have been exceeded. 
The CCTV footages can also be accessed and using Image processing the information about the crowd at that area can be predetermined before the user decides to visit the place. This will help in maintaining social distancing.
### III.	A chatbot for general FAQs regarding the situation.
Machine learning-enabled chatbots for contactless screening of COVID-19 symptoms and to answer questions from the public. The chatbot assesses known symptoms and answers questions about government policies. 

An additional feature we like to add is given below, though the implementation in the current scenario is hard and can be developed in the future.
### IV.	Reduce bottlenecks by providing time slots
One way to avoid unnecessary crowding is by proactively detecting mounting traffic as it forms and mitigating  risks. One way to do so is by assigning  time-slots for people  to go to a particular place .This will make sure that the number of people in a place would not exceed beyond what is mentioned. Here image processing can be used to identify and update the number of people currently present in a place. People will have the option to pre-book for a time slot and go there only during their assigned time. The number of people present in a place on a larger scale can be done using GPS tracking of phones.

## General Description

![architecture](https://github.com/NeomiSony/SocialDistancingApp/blob/main/Socialapppics/diag.png?raw=true)

 The solution is developed entirely on IBM Cloud using various Watson APIs namely Watson Assistant, Watson IOT platform and Watson Visual Recognition along with Node-RED. A database on Cloudant is required for storing the historical data of search location preferences and also the run time data. Node Red is a low-code development environment used for wiring the Watson and Cloudant components together. And finally we use the built in dashboard nodes that come with Node-RED to perform analysis on the data procured and give the crowd assessment at a particular location, alert beep of Covid positive patients nearby and a Chatbot for asking queries. This dashboard can be accessed by any user with the URL provided to access the Web Application or can be hosted as a Mobile Application for easier accessibility and use of the product.
 
 ## Technology Stack
The various software tools used in the proposed system are discussed in detail in this section.
### •	IBM Cloud 
The IBM Cloud platform is composed of multiple components that work together to provide a consistent and dependable cloud experience. Developers can use IBM services to create, manage, run and deploy various types of applications for the public cloud, as well as for local or on-premises environments. IBM Cloud supports various programming languages, such as Java, Node.js, PHP and Python. 
### •	Node Red 
Node-RED is a flow-based development tool for visual programming developed originally by IBM for wiring together hardware devices, APIs and online services as part of the Internet of Things. Node-RED provides a web browser-based flow editor, which can be used to create JavaScript functions. The Node-RED dashboard is an add-on module that lets you create live dashboards.
### •	Watson IoT platform
An IoT platform is a multi-layer technology that enables straightforward provisioning, management, and automation of connected devices within the Internet of Things universe. It basically connects your hardware, however diverse, to the cloud by using flexible connectivity options.
### •	Watson Visual Recognition
The Visual Recognition service uses deep learning algorithms to analyze images for scenes, objects, text, and other subjects.  Watson Visual Recognition makes it easy to extract thousands of labels from your organization's images and detect for specific content out-of-the-box. You can also build custom models to detect for specific content in images inside your applications.

### •	IBM Watson Assistant
Watson Assistant is IBM’s AI product that lets you build, train, and deploy conversational interactions into any application, device or channel. It provides customers with fast, consistent and accurate answers across any application, device or channel. This can be used for creating chatbots.

## Result:  
The final App is developed on Node-RED and visualized on the Node-RED Dashboard. Here we can choose the date of travel from the date picker and the location from the list of places provided. Depending on the crowd at the chosen location the visual recognition node performs image processing and classification and gives as a notification saying whether its safe or not to travel according to less or too much crowd respectively.
We have an alert message that warns us of people in close proximity from the device that’s connected to our device through bluetooth and the distance of the person near you. A link to a chatbot for Covid-19 related queries is also provided where it takes you to the chatbot earlier created on Watson Assistant and gives results according to the questions asked.
For further visualization of the crowd we can choose analyse which takes us to a page with images of the locations and by dragging the image url to the box and choosing analyse it gives us a table of all the objects detected in the image. If person is one of the classes detected we get the message saying too crowded.

![notif](https://github.com/NeomiSony/SocialDistancingApp/blob/main/Socialapppics/notif.png?raw=true)

![analyse](https://github.com/NeomiSony/SocialDistancingApp/blob/main/Socialapppics/analyse.png?raw=true)


![chatbot](https://github.com/NeomiSony/SocialDistancingApp/blob/main/Socialapppics/chatbot.png?raw=true)

## URL of our Project
https://node-red-qnayt-2020-09-25.eu-gb.mybluemix.net/ui/#!/0?socketid=caLZd27NBn95bWY9AAAs 

## Demo Video
https://youtu.be/WBizira81SM

## Implementation
The working along with screenshots from our project are given below-
### •	Proximity alert (Bluetooth)- 
For this feature we require Watson IOT Platform for detecting any close by devices. When bluetooth is turned on, the phone uses radio waves to figure out which other devices are nearby and the connected device information is sent as MQTT to Watson IOT platform. We use information from the Arogya Setu App to check if the connected device is that of a Covid positive patient and an immediate beep alert is sent to the user to warn them which is done with the help of Node-RED.

![iot](https://github.com/NeomiSony/SocialDistancingApp/blob/main/Socialapppics/iot.png?raw=true)
 
### •	Chatbot- 
The queries related to Covid can be asked by users on the Node-RED Dashboard URL provided or the Mobile Application with the help of Watson Assistant which is another Watson service available on the Cloud. It uses a Chatbot, also called Assistant to leverage industry leading AI capabilities to understand questions that the customers ask in natural language and uses machine learning models that are custom built from the data entered to deliver accurate answers in real time.


![assist](https://github.com/NeomiSony/SocialDistancingApp/blob/main/Socialapppics/assist.png?raw=true)

### •	Crowd Assessment(Location Based)- 
The CCTV footages of various locations are accessed and using the Watson Visual Recognition API we can perform image processing on the data obtained to determine the number of people at that location. Thus when a user decides to go out he/she can search for the location he/she wants to visit and get a clear idea of the crowd at that area. This will help him choose a different location with less people or go to the preferred location at a different time. GPS tracking can also be used as an additional feature for checking crowd at an area where CCTV is not available. The previous location preferences searched by the user can be stored on a Cloudant database to be accessed by Node-RED so that we can provide a more faster and user friendly method to perform searches.


![visual](https://github.com/NeomiSony/SocialDistancingApp/blob/main/Socialapppics/visuaise.png?raw=true)
 
### •	Node-RED Implementation- 
All the code required for our app is built using the nodes provided on Node-RED. The Visual recognition, Watson Assistant and Cloudant services were connected to Node-RED and used later. HTML and JavaScript were also used for the webpages and for some of the functions defined.

The below screenshots has the complete Node-RED code of our App.

![node1](https://github.com/NeomiSony/SocialDistancingApp/blob/main/Socialapppics/node1.png?raw=true)


![node2](https://github.com/NeomiSony/SocialDistancingApp/blob/main/Socialapppics/node2.png?raw=true)

## Conclusion:
As the Covid-19 situation kept worsening, countries around the world enforced strict lockdowns to combat the spread of the virus. However, lockdowns have a grave impact on a country's economy and extended lockdowns are not a viable option for the long term. Thus it is important  that we learn to live with the virus by following social distancing norms and mining proper hygiene. The features of the app inculcate various technologies and AI help with maintaining social distancing. The app can be used to predict the risk of infection in a particular area, send alerts when someone stands less than 6m radius when required, book slots of a particular store that has a limitation on the number of people allowed to enter at once. A chatbot is also available to ensure that any doubts or FAQs regarding this situation is addressed. The app, if used by many people, has the chance to help in reducing spread of the virus in a post lockdown world.

## Future Works:
●	Including a facemask detection feature to detect and alert individuals when facemasks are detected or not on an individual. 

●	Including a feature to give live updates about the number of people currently at the store.

●	A feature to give alerts to the user when the visitor limit has reached.

●	Expanding the project by visually representing object movement and hotspots on the app screen for selected location. 


## References:
•	https://nodered.org/docs/


•	https://youtu.be/3gxMBtvsRFo


•	https://youtu.be/YywNFisH7mo


•	https://www.ibm.com/watson/how-to-build-a-chatbot


•	https://developer.ibm.com/technologies/artificial-intelligence/patterns/detect-track-and-count-cars-in-a-video/

