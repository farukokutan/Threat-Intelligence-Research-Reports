# Network Settings for Using Tor with VM

The Tails operating system is designed to provide a secure and anonymous online experience. Default network settings enable users to connect to the internet while preserving their privacy. In this article, I will provide a general overview of the network settings in the Tails operating system.

### VMware Network Settings

![VM Network Settings Used for Tails](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V2.0/Tails-Network-Settings-1.png)

After installing the Tails operating system, you can choose how to connect to the network in the settings of your virtual server. There are five different types of connections:

1. **NAT (Network Address Translation):** Allows virtual machines to connect to the network with the host computer's IP address. Provides access to external networks but prevents direct access from external devices.
2. **Bridged:** Connects the virtual machine to the host computer's physical network. Allows direct communication with other devices.
3. **Host-Only:** Virtual machines can only communicate with the host computer and have no access to external networks.
4. **Custom:** Allows the user to define custom network configurations.
5. **LAN Segment:** Assigns virtual machines to a specific LAN segment, preventing communication with devices outside the segment.

### Tails Network Settings

Accessing network settings in the Tails operating system is straightforward. After completing the Tails installation, you can follow these steps:

1. **Using the Terminal:** Alternatively, you can open the terminal and use the **`ip a`** command to view existing network connections and IP addresses.
2. **Using the Menu for Network Settings:** Click on the "Network Settings" option in the menu on the Tails desktop. This option allows you to configure network connections and monitor network status.

**1. Using the Terminal**

For example, you can use the following command to display IP and MAC addresses in color-coded format:

```bash
ip a | grep -E --color=always "inet [^0-9.]+|[a-z]*:[0-9a-z]*+|[0-9]"
```

![VM Network Settings Used for Tails](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V2.0/Tails-Network-Settings-2.png)

**2. Using the Menu for Network Settings**

The "Network Settings" menu allows users to manage and configure network connections. It includes functions such as viewing existing connections, adding new connections, editing existing connections, checking network status, and managing network profiles. This menu is typically provided by the operating system or network management tools and makes it easy to manage network connections.

![VM Network Settings Used for Tails](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V2.0/Tails-Network-Settings-3.png)

![VM Network Settings Used for Tails](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V2.0/Tails-Network-Settings-4.png)

For example, by following the steps in this menu, I'm enabling 802.1x. 802.1x is an IEEE standard used for authentication and access control in wireless networks, and I prefer PEAP, the most secure authentication option. This process can be somewhat complex and require more technical knowledge, but it provides a more secure connection. Enabling this setting requires users to authenticate to access your network, enhancing protection against unauthorized access.

However, for you to use 802.1X, your network must also support this standard. Most home networks do not support 802.1X, so enabling this setting may make it difficult for you to connect to your network.

![VM Network Settings Used for Tails](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V2.0/Tails-Network-Settings-5.png)

![VM Network Settings Used for Tails](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V2.0/Tails-Network-Settings-6.png)

![VM Network Settings Used for Tails](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V2.0/Tails-Network-Settings-7.png)

In conclusion, the default settings in the Tails operating system provide a secure and anonymous connection for users. By choosing different options, you can create a more secure network and configure it according to your needs. For more information, you can refer to the Tails documentation and online resources.