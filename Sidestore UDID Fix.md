# SideStore UDID Fix for iOS 26.4+ 

For those who are having issues with iLoader and iOS 26.4+ regarding SideStore, here is a small tutorial on how to fix your pairing file.

# Explanation

The reason your pairing file is broken is due to a borked lockdown pairing file from the old versions of iLoader. In the newer versions of iLoader a new method of pairing was implemented, RPPairing. It is a more stable method of pairing compared to lockdown, and can never expire. The pairing also stays active when switching to cellular.

# Guide

1. First, make sure you have the latest version of iLoader installed (2.2.5 or newer). 
2. If you already have the latest iLoader installed, make sure you are logged in to your Apple ID. Scroll down and click "Delete Stored Pairing". 

Windows:
![image](/assets/iloader-1.png)
Linux:
![image](/assets/iloader-3.png)
Mac:
![image](/assets/iloader-4.png)
This will remove any existing pairing file, but you will have to pair your phone again. This will get rid of the cached lockdown pairing.
3. After deleting the stored pairing, go to Settings, click General, scroll down to "VPN and Device Management", click your email under "Developer App", and click "Delete Apps". 

<img src="/assets/image0.jpg" width="500" height="400">
<img src="/assets/IMG_1905.jpg" width="500" height="400">
    
Go back to iLoader, pair your phone again, and install SideStore (Stable). 
4. Once SideStore is installed, test an app to see if it installs correctly. If it does, your pairing file is fixed and you can use SideStore as normal. If need be, change the anisette server to 'Macley'.

<img src="/assets/sidestore-2.png" width="500" height="400">


# Extra Steps (if the steps above do not work)

1. Open LocalDevVPN, find the Tunnel IP address.

<img src="/assets/localdevvpn-1.png" width="500" height="400">
2. Go to the SideStore settings, find VPN Configuration, and set the Device IP to the Tunnel IP address you found in LocalDevVPN.

<img src="/assets/sidestore-1.png" width="500" height="400">
3. Refresh your apps like normal.
