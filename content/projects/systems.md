---
title: "Systems Communication"
image: "images/projects/systems/systemsimage.png"
isProject: true
---

The Systems software sub-team has the main goal of facilitating communication between the driver and the vehicle. This is completed by using the User Interface to exchange information with the driver and a CAN bus to exchange information with the electrical components on the vehicle. Information sources from the vehicle to the driver may include: car battery, speed, proximity sensor data, and more. Networking of this information from all sources to their appropriate destinations was completed using the open-source library ZeroMQ. This is a concurrency framework which allows for concurrent, socket-based communication from a variety of sources to the User Interface and vice versa.

The necessary hardware to run the System’s core will consist of a Raspberry Pi Compute Module 4 along with the corresponding I/O Board. These will be hidden behind the dash where the User Interface screens will be visible. The close-proximity of the Systems hardware to the User Interface hardware is necessary as these will need to be concurrent programs which seamlessly integrate with each other. This project is an extremely important component of the process of converting EVs due to the removal and addition of critical dashboard features due to the gas engine being replaced with a battery and motor. New critical information, such as battery life, must be added for the driver’s safety. In order to have this vital data displayed, communication must be efficient and reliable between the vehicle’s components and the User Interface.

![Full stack demo](/images/projects/systems/front-to-back-communication.png)

The Systems communication sub-team has been able to achieve communication between the User Interface and the System’s core. Simultaneously, members focussing on CAN bus communication have also been able to retrieve and display data from a sensor— one of the potential sources of information from the vehicle to be displayed on the User Interface. Once data from the CAN bus can be read and parsed by the System’s core, the project will be virtually complete. It is estimated that the Software Team will accomplish this by December 2021.
