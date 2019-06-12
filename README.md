# iotedge_v2_snap
Snapcraft files to create a snap for the Microsoft Azure IoT Edge solution (https://github.com/Azure/iotedge)

Create new snap:
1. Run snapcraft in the root directory

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
