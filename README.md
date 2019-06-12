# iotedge_v2_snap
Snapcraft files to create a snap for the Microsoft Azure IoT Edge solution (https://github.com/Azure/iotedge)

Create new snap:
1. Prerequisites:
    enable lxd
        sudo addgroup --system lxd
        sudo adduser $USER lxd
        sudo snap install lxd
        # restart your desktop session so that the lxd group membership is applied
        lxd init
        # press enter to accept all the default options that it asks you

2. Run snapcraft in the root directory
    snapcraft cleanbuild # cooking with gas!

Install snap:
1. Download the released snap file
2. Install using following command: 
```console
    sudo snap install --devmode iotedge_v2-preview_amd64.snap
```

Run Iotedge
In the current version it is not possible yet to run iotedge as a systemd service. Run following command to execute the iotedge daemon
```console
  sudo iotedge.iotedged
```
