# NIC
Open "Control Panel\Network and Internet\Network Connections"
Open the adapter's Properties.
Disable the NDIS6 virtualbox by unticking.
Click Ok
Right-click adapter->disable.
Open the adapter's Properties again.
Enable the NDIS6 virtualbox by ticking.
Click Ok
Right-click adapter->enable.
# VB Guest
wget https://download.virtualbox.org/virtualbox/7.1.0/VBoxGuestAdditions_7.1.0.iso -P /tmp
sudo mount -o loop /tmp/VBoxGuestAdditions_7.1.0.iso /mnt
sudo systemctl daemon-reload
sudo sh /mnt/VBoxLinuxAdditions.run