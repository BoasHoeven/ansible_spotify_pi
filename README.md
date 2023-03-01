# Setup commands
```
sudo apt-get update && sudo apt-get upgrade -y && sudo apt install ansible git -y
sudo reboot
git clone https://github.com/BoasHoeven/ansible_spotify_pi.git
```

Update the config file with credentials. Then run the following cmds:

```
ansible-galaxy collection install -r requirements.yml
ansible-playbook main.yml
```

> **If running locally on the Pi**: You may encounter an error like "Error while fetching server API version". If you do, please either reboot or log out and log back in, then run the playbook again.
