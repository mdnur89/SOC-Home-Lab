Download
Go to the official site.

Download the last stable version of the community edition.

VirtualBox Settings
Create a new virtual machine.

![alt text](images/image.png)

![alt text](images/image2.png)

![alt text](images/image3.png)

![alt text](images/image4.png)

![alt text](images/image5.png)

![alt text](images/image6.png)

Go to the VM properties.

In Network tab, activate 3 adapters.

Making note of the MAC Addresses of each adapters will be useful for future actions. This will be the RED CARD. (external network)

![alt text](images/image7.png)

This will be the GREEN CARD. (internal network)

![alt text](images/image8.png)

This will be the orange CARD. (dmz)

![alt text](images/image9.png)

Launch the VM. It will ask you which ISO Virtualbox must mount on the VM, load the pfsense one.

![alt text](images/image10.png)

Installation:

select "install"

![alt text](images/image11.png)

next,
-Select your keymap
-Use the default partition (we're in a lab, we just need a firewall)
-Proceed with installation (no miror, no encrypt, nothing)
-Wait until the installation is complete

->>Do not load manual configuration.<<-

![alt text](images/image12.png)

->>Do not load manual configuration.<<-
Then reboot the VM.

Configuration:
Now, the server is powered on with the new system.

![alt text](images/image13.png)

Select 1 to configure interfaces.

![alt text](images/image14.png)

We can see the MAC Addresses. Remember, we recommended to make a note of the MAC addresses. It is always helpful to have/know them.

-Select the RED INTERFACE for WAN
-Select the GREEN INTERFACE for LAN
-Select the last one (ORANGE) for DMZ

![alt text](images/image15.png)

Confirm!

![alt text](images/image16.png)

-Select 2 to configure the IP address
-Leave the WAN interface as DHCP
-Select 2 to change the LAN interface
-Assign the IP and subnet you want, the gateway must be "none" !

AND THATS PART 1 DONE.
