1. install Python 3.11 on Ubuntu 24.04
  
```
    sudo add-apt-repository ppa:deadsnakes/ppa
    sudo apt update
    sudo apt install python3.11
    sudo apt install python3.11-venv
```

2. create venv and install requirements.txt 

```
    python3.11 -m venv myenv
    source myenv/bin/activate
    pip3 install -r requirements.txt
```


3. create common_config_local.json

```
   cd ./network_gym_client
   cp ./common_config.json ./common_config_local.json
```

4. update "server_ip" and "server_port" in common_conig_local.json as needed 


5. run the example python3 script for celllular RAN slicing (https://intellabs.github.io/networkgym/environments/mx_network_slicing/cellular_network_slicing.html#cards-mx-cellular-slicing) 

```
    python3 start_client_slicing.py 
```