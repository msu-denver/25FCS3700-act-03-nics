# Overview 

The goal of this activity is to identify and examine the network interfaces available on your computer. 

# Instructions 

In this activity, you will use Python’s [netifaces](https://pypi.org/project/netifaces/) package to discover the link-layer network interfaces available on your computer. For each interface detected, your code will display its corresponding MAC address.

Create and activate a Python virtual environment. Next, install the netifaces package. 

Open [src/link_layer.py](src/link_layer.py). Locate and complete the single TODO in the code to list all interfaces and display their MAC addresses.

Compare the output of your Python script with the network interface information displayed by your operating system. For example, if you have a Mac you can list your NICs using **About - System Report - Network**. 

Your laptop computer may show multiple NICs because modern systems often include both physical and logical (virtual) interfaces. For example, my MacBook Pro shows the following NICs: 

```
en0 ea:8c:3a:c5:15:3d
en1 36:4a:68:cd:26:40
en2 36:4a:68:cd:26:44
en3 96:01:17:ac:67:42
en4 8c:04:ba:98:4c:cc
en5 96:01:17:ac:67:43
```

* en0 – Typically the built-in Wi-Fi interface.
* en1, en2 – Could be additional physical interfaces like Ethernet (if using a USB-C adapter or dock), or older hardware like Bluetooth PAN.
* en3, en4, en5 – Often created by Thunderbolt docks, USB Ethernet adapters, or virtual interfaces from software like VPNs or virtualization tools (e.g., Parallels, Docker, VMware).
