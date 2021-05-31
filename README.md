---
layout: home
permalink: index.html
repository-name: e14-3yp-Control-System-for-Heliostat-Solar-Power-Plants
title: Control System for Heliostat Solar Power Plants
---
# Control System for Heliostat Solar Power Plants

---
## Team
-  E/14/233, NIROSHANA T.M.T., [e14233@eng.pdn.ac.lk](mailto:e14233@eng.pdn.ac.lk)
-  E/14/314, SENANAYAKA S.M.M.K.S , [e14314@eng.pdn.ac.lk](mailto:e14314@eng.pdn.ac.lk)
-  E/14/322, SENEVIRATHNE S.D., [e14322@eng.pdn.ac.lk](mailto:e14322@eng.pdn.ac.lk)

## Table of Contents
1. [Introduction](#introduction)
2. [Solution Architecture](#solution-architecture )
3. [Links](#links)

---

## Introduction

This is a system which focus sunlight into a one point in a solar tower and heat up the salts in it upto higher temperatures and then use them to store heat energy and produce steam and generate electricity. These systems make it possible to supply power even when the sun is down because of the stored heat energy. In these power plants, array of flat movable mirrors called heliostats are used to focus sunlight into a collector tower to heat salts and generate electricity through steam turbines. This is seen as  a viable solution for renewable energy.

Angle of heliostat is very critical in these solar power plants since the temperature of the tower will be significantly rely on the concentration of sunlight focused on it.

## Solution Architecture

CO321 - The position of the sun is calculated by the local server in the solar tower and will be broadcast to the network via WiFi interface. Then the other nodes (heliostats) receives data and adjust them according to their relative position and give the control signals to the motors to rotate the heliostats. Initial inclination of the heliostats will be sensed through a gyroscope. So after a successful turn a feedback signal will be sent to the local server which could be used to sense malfunctions.

 

CO324 - Usually these farms has nearly 2000 heliostats pointing one point. So sending a feedback to local server could induce a network conjunction. Data from the local server will be sent to the centralized server in real time or in short intervals from many farms owned by the same company throughout the country. So the network traffic which could occur in the systems will be considered in the design and it will be designed to minimize the drawbacks and control the overall MO of the system. Also the monitoring system can be used for maintenance scheduling by getting status feedbacks from the equipments, which adds an important feature to the implementation from adding network aspect.

 

CO325 - The feedback data sent from local servers of the farms to the centralized server are sent as encrypted data as this implementation mainly focuses on R&D and the collected data is a valuable asset and they have a market value. Therefore, it needs to be encrypted and security becomes a key aspect in the implementation. Also the signals sent to each node is encrypted as outside parties can manipulate nodes to reduce the efficiency of the system by changing direction of the heliostats by giving wrong feedbacks.



## Links

- <a href = "https://github.com/cepdnaclk/e14-3yp-Control-System-for-Heliostat-Solar-Power-Plants" target = "_blank"> Project Repository </a>
- <a href = "https://cepdnaclk.github.io/e14-3yp-Control-System-for-Heliostat-Solar-Power-Plants/" target = "_blank">Project Page</a>
- <a href = "http://www.ce.pdn.ac.lk/" target = "_blank">Department of Computer Engineering</a>
- <a href = "https://eng.pdn.ac.lk/" target = "_blank">University of Peradeniya</a>


[//]: # (Please refer this to learn more about Markdown syntax)
[//]: # (https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

