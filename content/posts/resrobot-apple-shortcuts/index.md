---
title: "Resrobot Apple Shortcuts"
date: 2023-07-14T09:51:39+02:00
---

During my vacation, I had the opportunity to delve into Apple Shortcuts and discover its potential for enhancing my daily routines. In particular, I found a practical application for Apple Shortcuts in obtaining transit departure information from a specific stop as soon as I leave an area. In this blog post, I'll provide a brief overview of Apple Shortcuts and explain how I used it, alongside the "ResRobot API" from [trafiklab.se](https://www.trafiklab.se/api/trafiklab-apis/resrobot-v21/), to solve this problem efficiently. Additionally, I'll share the two shortcuts I created for this purpose and provide the necessary resources to implement them.

**What is Apple Shortcuts?**  
Apple Shortcuts is a powerful automation app available across the complete Apple ecosystem, including iOS devices, iPadOS, and macOS. It allows users to create custom workflows by connecting different actions across various apps and services. These workflows, known as shortcuts, can be triggered manually or automatically to streamline repetitive tasks and simplify complex actions.

{{< figure src="images/apple-shortcuts.png" width="95%" caption="Apple Shortcuts are made for non programmers and the interface is contained by drag and droppable actions." alt="Screenshot of the Apple shortcuts application, containing 3 actions tied together." >}}

One of the challenges I often faced was keeping track of transit departure times from a specific stop, such as knowing when the next bus departs as soon as I leave work. This information is crucial for planning my commute and ensuring I catch the appropriate transit at the right time.

**Apple Shortcuts and ResRobot API**  
To address this problem, I turned to Apple Shortcuts and leveraged the ResRobot API from trafiklab.se, a valuable resource for transit information. ResRobot covers all public transportation in Sweden, providing comprehensive data across the country's transit network. By combining Apple Shortcuts with ResRobot, I was able to create a seamless workflow that provided me with real-time departure updates for my desired stop, regardless of the location in Sweden.

**The Shortcuts**  

_Helper Shortcut: Finding the Stop ID_  
The first shortcut I created is a helper shortcut designed to help users identify the unique ID of the stop they want to monitor. By inputting relevant information, such as the stop name or location, this shortcut interacts with the ResRobot API to retrieve the corresponding stop ID.

_Departure Updates Shortcut: Getting Upcoming Departures_  
The second shortcut is the core component that retrieves upcoming departure information based on the stop ID obtained from the helper shortcut. It communicates with the ResRobot API and fetches the latest transit departure data, providing you with timely updates on when the next bus, train, or other modes of transportation will depart.

{{< figure src="images/departure-notification.png" width="95%" caption="A notification sent by the Departure Updates Shortcut." alt="A screenshot of the notification, saying that bus line 4 arrives in 6min, 14min and 23min" >}}

To implement these shortcuts, you'll need to acquire an API key from trafiklab.se, which is freely available. Once you have the API key, you can download and install the shortcuts using the provided iCloud links:

* [Helper Shortcut](https://www.icloud.com/shortcuts/ba798fd2d47f4f1dbe00891b3b0ff333)
* [Departure Updates Shortcut](https://www.icloud.com/shortcuts/54e99ecb46a84aeabce3811a54311d75)

**Automation Possibilities**  
One of the remarkable features of Apple Shortcuts is its ability to connect with various automation triggers. This means you can integrate shortcuts with different types of actions, such as when you leave a specific area, arrive at a location, or even at a specific time of day. By exploring the automation options within the Shortcuts app, you can customize your workflows to perfectly suit your needs and optimize your daily routines.

By harnessing the power of Apple Shortcuts and integrating the ResRobot API, I was able to streamline the process of obtaining transit departure updates from a specific stop. Whether you're leaving work, heading home, or navigating through any other routine transit scenario, these shortcuts can save you time and provide you with the information you need at your fingertips. Try them out and experience the convenience of real-time transit updates tailored to your needs, anywhere in Sweden.
