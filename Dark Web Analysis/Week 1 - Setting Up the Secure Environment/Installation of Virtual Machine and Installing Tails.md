# Installation of Virtual Machine and Installing Tails

Virtual machines are machines installed on operating systems available on physical computers or servers through virtualization software, which can utilize the hardware and resources of the physical machine in a limited manner. Through this virtualization process, users can run multiple virtual machines on a single physical machine and install independently operating systems and applications on each.

The most commonly used and often recommended virtualization software for personal computers are:

1. VMware Workstation
2. Oracle VM VirtualBox

### Steps for Installing VMware Workstation

You can easily download VMware Workstation software, the simple and non-commercial free product [VMware Workstation Player](https://www.vmware.com/products/workstation-player.html), and the powerful feature-rich paid product [VMware Workstation Pro](https://www.vmware.com/products/workstation-pro/workstation-pro-evaluation.html) from VMware's official website.

I have downloaded the latest version, [VMware Workstation Pro](https://www.vmware.com/products/workstation-pro/workstation-pro-evaluation.html) version 17.5.1.

When you click on the download link on the website, the download process starts directly. When we run the downloaded file, a User Account Control (UAC) window opens asking whether to allow VMware to make changes to your device. We click the "Yes" button to continue the installation.

![VMware-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/VMware-Installation.1.png)

After granting this permission, VMware makes several changes, and then the VMware Workstation Pro Installation Wizard opens. The steps at this stage are quite simple; we can install the software by clicking "Next" in the windows that open.

The installation windows in order:

<center>

![VMware Workstation Pro Installation Wizard initial step](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/VMware-Installation.2.png)  
Img 1: VMware Workstation Pro Installation Wizard initial step

![Acceptance step of the End User License Agreement](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/VMware-Installation.3.png)
Img 2: Acceptance step of the End User License Agreement

</center>



![VMware-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/VMware-Installation.4.png)

In the "User Experience Settings" step of VMware Workstation Pro installation, it concerns checking for product updates and the VMware Customer Experience Improvement Program. The options in this step are optional, and you can proceed with the default settings.

![VMware-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/VMware-Installation.5.png)

In the "Shortcuts" step of VMware Workstation Pro installation, we can choose to create a shortcut in the start menu and on the desktop.

<center>

![Ready to complete the VMware Workstation Pro installation step](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/VMware-Installation.6.png)
Img 3: Ready to complete the VMware Workstation Pro installation step

</center>

![VMware-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/VMware-Installation.7.png)

In the final step of the Installation Wizard, a license key is requested. Since we will use the trial version, we click the "Finish" button to complete the installation.

Finally, when we run the software, the Workstation Pro 17 screen appears.

![VMware-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/VMware-Installation.8.png)

Additionally, since the installation of VMware Workstation Pro and VMware Workstation Player progresses similarly, I haven't prepared a separate installation document for Player.

<center>

![Interface screens of VMware Workstation Pro and VMware Workstation Player](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/Pro-vs-Player.png)
![Interface screens of VMware Workstation Pro and VMware Workstation Player]([images](/releases/download/V1.0/pro-vs-player.png)/Pro-vs-Player.png)
Img 4:Interface screens of VMware Workstation Pro and VMware Workstation Player

</center>

### Steps for Installing Tails

Tails, compared to other Linux operating systems, is a Linux operating system focused on privacy and anonymity. Tails can be installed on a USB flash drive and used on any computer. Tails routes all internet traffic through the Tor network, has powerful encryption tools and applications, and can reset every session to not retain user's private data. Therefore, it is a reliable option to enhance digital security and ensure online privacy.

The [official Tails website](https://tails.net/install/index.en.html) provides documentation on how to install Tails on Windows, MacOS, Linux, and via Terminal. Additionally, the documentation includes information on [running Tails in virtual machines](https://tails.net/install/vm/index.en.html), which is what we will do today.

![Tails-Web](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/Tails-Web.1.png)

Step 1) Firstly, we download the latest version. I downloaded version 6.0 while preparing this guide.

![Tails-Web](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/Tails-Web.2.png)

Step 2) As seen in the document, there is a simple installation process. After verifying and obtaining approval in the verification area in step 2, we open the virtualization software we will use for the installation process.

![Tails-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/Tails-Installation.1.png)

Step 3) Since we will perform a new installation in the first step, we click the "Create a New Virtual Machine" button on the main screen. This will start the virtual machine creation wizard. Since we don't need to make a detailed setup at this stage, we proceed by selecting the "Typical (recommended)" option.

<center>

![Tails-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/Tails-Installation.2.png)
Img 5: Wizard window for creating a new machine installation

</center>

Step 4) In the next step, to work with the ISO file we downloaded earlier, let's select "Installer disk image file (ISO)". By clicking the "Browse" button, navigate to the location of the downloaded ISO file and select the "tails-amd64-6.0.iso" file. Then proceed.

<aside>
📌 The option we choose here helps us to perform an easy installation. If we want to perform a customized installation, select the "I will install the operating system later" option during the creation process. This will skip the Easy Install process and allow you to customize settings during installation.
</aside>

<center>

![Tails-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/Tails-Installation.3.png)
Img 6: Selection of the file where the operating system will be installed

</center>

Step 5) At this stage, considering that the latest version of Tails is based on Debian 12, let's select the version number corresponding to Debian 12. Then proceed.

<center>

![Tails-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/Tails-Installation.4.png)
Img 7: Selection of the operating system type and version

</center>

Step 6) At this stage, we need to choose a name for our virtual machine and select where the virtual machine files will be stored. After completing the necessary information, proceed.


<center>

![Tails-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/Tails-Installation.5.png)
Img 8: Selection of the directory where the virtual machine will be saved

</center>

Step 7) At this stage, we determine the disk size our virtual machine will use. I'm allocating 30 GB of space considering that my system has a 480 GB SSD and taking into account the available space in the system, but you can allocate more or less space. According to my research, the ideal disk size for Tails is 20 GB. However, if it will be used continuously and you have sufficient free space, I recommend allocating 30 - 40 GB. Also, we prefer the "Store virtual disk as a single file" option. In general, selecting the single file option is better for performance and simpler management, so in most cases, choosing the "Store virtual disk as a single file" option would be reasonable.

<center>

![Tails-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/Tails-Installation.6.png)
Img 9: Determination of the disk capacity to be used by our virtual server

</center>

Step 8) We are in the final stage of the installation. At this point, optionally, we can increase or decrease some hardware specifications of our virtual server.

<center>

![Tails-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/Tails-Installation.7.png)
Img 10: Final state of the information and hardware specifications of the virtual server, creation of the virtual machine

</center>

I'm increasing the memory size from 2048 MB to 4096 MB. We can change these values later if we want. Also, in the network adapter selection, I prefer the "NAT" mode. This mode allows our virtual machine to share internet access with your host computer but cannot communicate directly with other devices. This can help your virtual machine connect to the internet more securely.

<center>

![Tails-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/Tails-Installation.8.png)

![Tails-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/Tails-Installation.9.png)

</center>

Step 9) After determining all the information and hardware specifications, we finalize the installation wizard of our virtual server with the "finish" button and can start the virtual server.

<center>

![Tails-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/Tails-Installation.10.png)

</center>

Step 10) The options "Tails" and "Tails (Troubleshooting Mode)" represent different boot modes on the Tails operating system. The "Tails" option boots the Tails operating system for normal daily use, while the "Tails (Troubleshooting Mode)" option boots the troubleshooting mode of Tails for troubleshooting. Since there are no problems, we continue with the normal boot option "Tails".

<center>

![Tails-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/Tails-Installation.11.png)

![Tails-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/Tails-Installation.12.png)

</center>

Step 11) In the window that opens, in the "Language and Region" section of the Tails operating system welcome screen, you can select your language and keyboard layout. Additionally, you can set an administrative password through additional settings. At this stage, I am only setting an administrative password and leaving other settings at their default values.

<center>

![Tails-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/Tails-Installation.13.png)

</center>

Step 12) At this stage, two options regarding the tor connection are provided. In most cases, selecting the **"Automatically configure the Tor connection"** option will be sufficient, but if using Tor appears suspicious to someone monitoring your internet connection, you may need to go unnoticed, so it would be more appropriate to select the more reliable option **"Hide to my local network that I'm connecting to Tor"**. I am continuing with the **"Automatically configure the Tor connection"** option for this step.

<center>

![Tails-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/Tails-Installation.14.png)

![Tails-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/Tails-Installation.15.png)

</center>

Step 13) And now Tails is ready to use. We can start using it by launching the Tor Browser.

<center>

![Tails-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/Tails-Installation.16.png)

![Tails-Installation](https://github.com/farukokutan/Threat-Intelligence-Research-Reports/releases/download/V1.0/Tails-Installation.17.png)

</center>

If you query your IP address and see a Tor exit node IP address, it means your internet traffic is routed through the Tor network, and your real IP address is hidden. This allows Tor users to browse the internet anonymously and reduce the risk of tracking.

Your operations have been completed smoothly and you have successfully installed Tails and connected to the Tor network. This will allow you to browse the internet anonymously and securely.

[Tails - Documentation](https://tails.net/doc/index.en.html)

[Computer Security with Tails - Free Software Association Security Guide](https://guvenlik.oyd.org.tr/cihaz_guvenligi/tails.html#tails-kullanımı)
