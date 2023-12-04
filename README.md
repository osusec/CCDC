# Easily deploy security checks to servers

### Installation

In order to properly run this, you need to install ansible:

With package manager:
```
sudo apt-get install ansible
```
With pip:
```
pip install ansible
```

You will also need sshpass:
```
sudo apt-get install sshpass
```

### Usage

1. Add `keys/` folder `mkdir keys`
2. Generate public and private keys and place them in the `keys/` folder 
3. Add a password in the `keys/pass.txt` file.
4. Modify inventory file with hosts and default username/password
5. Run the playbook: `ansible-playbook ansible_defense.yml -i inventory.ini`
