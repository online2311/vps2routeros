# vps2routeros

This script will wipe your current OS then install RouterOS on the target computer without requiring physical access. It has been proven to work with a wide range of VPSs.


## WARNING

> Your warranty is now void. I am not responsible for bricked devices, dead HDDs and SSDs, unreplied tickets, thermonuclear war, or you getting fired because your device is hacked to mine bitcoin. Please do some research if you have any concerns about this script before using it! YOU are choosing to make these modifications, and if you point the finger at me for messing up your device, I will laugh at you.

* **PLEASE READ THIS DOCUMENTATION THROUGHLY BEFORE RUNNING**
* CAUTION: ALL DATA ON YOUR DEVICE WILL BE LOST INSTANTLY! There is no way to get them back.
* Please make a backup of your existing network configuration prior to running this in case of any problem
* If you use IPv6, remember your gateway link-local address too
* Please SET AN PASSWORD IMMEDIATELY after installation
* Please UPDATE IMMEDIATELY after installation

## Usage

### Requirements

The target device:

* is amd64 (sometimes called x86_64) architecture
* is a physical device or a full-virtualized VM
* runs Ubuntu 16.04 or higher (we recommend Ubuntu 16.04; other distros are not tested)

### Running the script

1\. download this script to the target computer:

```shell
# use wget
wget https://raw.githubusercontent.com/online2311/vps2routeros/master/vps2routeros.sh

# or use curl
curl -L https://raw.githubusercontent.com/online2311/vps2routeros/master/vps2routeros.sh -o vps2routeros
```

2\. Use any text editor to open the script, change the default config if needed

3\. run it:

```shell
chmod +x ./vps2routeros
sudo ./vps2routeros
```

4\. Set a password:

Login with WinBox or HTTP or SSH using username `admin` and an empty password, then change the password.
