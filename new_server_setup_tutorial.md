# Initial setup tutorial

1. Connect device to keyboard and monitor
2. Instal ubuntu server and configure it
3. Check your network devices with `ip a` or `ip link`
4. Configure network connection by creating DHCP config

    ```bash
    ls /etc/netplan # if empty then
    sudo nano /etc/netplan/01-netcfg.yaml
    ```

    paste it there changing name of the network device

    ```yaml
    network:
      version: 2
      ethernets:
        eno1:
          dhcp4: true
    ```
  
5. Now you can unplug it and connect it to the ethernet, then turn it on
6. In router dashboard check the IP of this new device
7. Connect to it via ssh
8. Clone this repo

    ```bash
    git clone https://github.com/nizwant/home_server_setup.git
    ```

9. Run startup script, it downloads and setups docker and downloads any updates
