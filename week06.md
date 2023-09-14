# Week 6 | WIRELESS NETWORKS

## Task 1. View Wi-Fi Details

I have configured the WifiTools module first to view the Wi-Fi details of my laptop.


![instalWifiTool](./images/instalWifiTool.png)


Showed the list of commands available in the WifiTools module and showed the help for the Get-WifiState command

![Get-WifiState](./images/Get-WifiState.png)

Check the basic Wifi information using the Show-WifiState command

![Show-WifiState](./images/Show-WifiState.png)

  I have collected different APs: BSSID, frequency band, channel, data rate by using Scan-WifiAPs command.

 ![Scan-WifiAPs](./images/Scan-WifiAPs.png)


 I used Show-WifiInterface to collect more wifi information.

Wifi Profile Name: WiFi-54CF-5G

 ![Show-WifiStateInterface](./images/Show-WifiStateInterface.png)

I used Get-WifiLog | Select -First 10 command to get the first most recent 10 log entries of events that occurred.

 ![First10](./images/First10.png)

## Task 2. Use Wi-Fi Access Point

 ![ArcherC6](./images/ArcherC6.png)


When designing a Wi-Fi network, there are many important settings that should be considered to ensure optimal performance and security. Here are a few them: 

1. Network Name (SSID): To prevent confusion with other adjacent Wi-Fi networks, the network name or SSID should be carefully chosen. It is advised to choose a distinctive name that is simple to remember and difficult to guess.

2. Encryption Method: How data is protected during transmission between networked devices depends on the encryption technique used. The most recent encryption standards, like WPA3, are advised to offer the best level of security.

3. Authentication Method: How devices connect to the Wi-Fi network is based on the authentication technique. The adoption of a robust authentication technique, such as WPA2-Enterprise, which necessitates the input of a special username and password by users in order to access the network, is advised.

4. Channel Selection: Wi-Fi networks use particular radio frequency channels to operate, and selecting the best channel can greatly enhance performance. To find the least crowded channels in the vicinity and choose the one with the least interference, it is advised to utilise a Wi-Fi analyser tool.

5. Quality of Service (QoS): QoS settings allow you to prioritize certain types of traffic on the network, such as video or voice data, to ensure smooth performance. It's recommended to enable QoS settings and prioritize critical applications over less important ones.

6. Guest Access: Guest access settings allow you to provide Wi-Fi access to visitors without giving them full access to your network. Enabling guest access and setting up a separate network with its own security configurations and constrained access to internal resources are both recomoneded..


## Learning Reflection

This week I learned about wireless and wired networks, spectrum, channels, frequencies, and common wireless technologies. I also learned about wireless LAN standards and typical WiFi networks and design issues.

While this turoril doing, I was getting "The Module Could Not Be Loaded" error message when I am tryoing to command Show-WifiState command. To fix it I follwed following steps.

1.Get-ExecutionPolicy

2.Set-ExecutionPolicy -ExecutionPolicy Unrestricted -Scope Process

3.Set-ExecutionPolicy -ExecutionPolicy Unrestricted -Scope CurrentUser

## Extra Resources
1.https://www.tp-link.com/au/support/emulator/
  
2.https://www.easy365manager.com/the-module-could-not-be-loaded/
